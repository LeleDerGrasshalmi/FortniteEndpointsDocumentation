## EGS Platform Service - Slug Mapping

URL: https://egs-platform-service.store.epicgames.com/api/v1/egs/mappings/:slug \
Method: GET \
Auth Required: No

## Query Parameters

`country`: (required) ISO 3166 - Alpha 2 Code <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en'

## Path Parameters

`slug`: The Offer Url slug, e.g. `fortnite` for Fortnite or `fortnite--uefn` for UEFN

---

_Example Response_

```json
{
  "__typename": "OfferMapping",
  "modules": {
    "pageOffers": [
      {
        "__typename": "MappingPageOfferModule",
        "categories": [
          "games",
          "games/edition",
          "games/edition/base",
          "attention/in-app-purchases/supported",
          "applications"
        ],
        "effectiveDate": 1505912400000,
        "offerId": "09176f4ff7564bbbb499bbe20bd6348f",
        "sandboxId": "fn",
        "store": "EGS"
      }
    ]
  },
  "productId": "prod-fn",
  "sandboxId": "fn",
  "slug": "fortnite"
}
```
