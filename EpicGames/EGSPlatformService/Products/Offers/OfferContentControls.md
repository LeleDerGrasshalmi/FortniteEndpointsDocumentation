## EGS Platform Service - Product Offer Content Controls

URL: https://egs-platform-service.store.epicgames.com/api/v1/private/egs/products/:productId/offers/:offerId/content-controls \
Method: GET \
Auth Required: Yes

## Query Parameters

`country`: (required) ISO 3166 - Alpha 2 Code <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`store`: (required) valid Catalog Service Stores, e.g. `EGS`

## Path Parameters

`productId`: self explaining, e.g. `6f3979ff608f42e286c83507a69b27f5` for Honkai Star Rail <br/>
`offerId`: self explaining, e.g. `0728f2df169d4abca07e83a452b1ef6c` for the Honkai Star Rail Main Offer

---

_Example Response_

```json
{
  "__typename": "OfferContentControl",
  "contentControl": "NoGate"
}
```
