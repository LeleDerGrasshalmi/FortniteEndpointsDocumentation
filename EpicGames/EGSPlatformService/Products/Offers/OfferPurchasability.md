## EGS Platform Service - Product Offer Purchasability

URL: https://egs-platform-service.store.epicgames.com/api/v1/private/egs/products/:productId/offers/:offerId/purchasability \
Method: GET \
Auth Required: Yes

## Query Parameters

`country`: (required) ISO 3166 - Alpha 2 Code <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`store`: (required) valid Catalog Service Stores, e.g. `EGS`

## Path Parameters

`productId`: self explaining, e.g. `prod-fn` for Fortnite <br/>
`offerId`: self explaining, e.g. `09176f4ff7564bbbb499bbe20bd6348f` for the Main Fortnite Offer

---

_Example Response (unavailable)_

```json
{
  "__typename": "OfferPurchasability",
  "purchasability": [
    {
      "purchasable": "Unavailable",
      "purchaseStateEffectiveDate": 1715511180000,
      "reason": "InLibrary"
    }
  ]
}
```

_Example Response (available)_

```json
{
  "__typename": "OfferPurchasability",
  "purchasability": [
    {
      "purchasable": "AvailableToClaim",
      "purchaseStateEffectiveDate": 1715511360000
    }
  ]
}
```
