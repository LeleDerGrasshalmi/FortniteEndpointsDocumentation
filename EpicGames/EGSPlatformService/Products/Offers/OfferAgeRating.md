## EGS Platform Service - Product Offer Age Rating

URL: https://egs-platform-service.store.epicgames.com/api/v1/egs/products/:productId/offers/:offerId/age-rating \
Method: GET \
Auth Required: No

## Query Parameters

`country`: (required) ISO 3166 - Alpha 2 Code <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`store`: (required) valid Catalog Service Stores, e.g. `EGS`

## Path Parameters

`productId`: self explaining, e.g. `7c0a8a40ba4a47dd899eed51a8fbc3fe` for Rogue Company <br/>
`offerId`: self explaining, e.g. `36bfbc7a0b664a2891c68dc947922469` for the Rogue Company Main Offer

---

_Example Response_

```json
{
  "__typename": "AgeRating",
  "ageGate": {
    "gate": "age-gate"
  },
  "ageRating": {
    "ageControl": 17,
    "contentDescriptors": [],
    "interactiveElements": [],
    "ratingImage": "https://cdn1.epicgames.com/gameRating/gameRating/ESRB_RP17_136_136x136-d2458f66245ec23152ff2846c7b6de7e",
    "ratingSystem": "ESRB",
    "title": "RATING PENDING"
  }
}
```
