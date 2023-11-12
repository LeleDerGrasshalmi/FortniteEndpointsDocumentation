## EGS Platform Service - Product Offer Age Rating

URL: https://egs-platform-service.store.epicgames.com/api/v1/egs/products/:productId/featured-offers/add-ons \
Method: GET \
Auth Required: No

## Query Parameters

`count`: (required) element count to return <br/>
`country`: (required) ISO 3166 - Alpha 2 Code <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`start`: (required) start index <br/>
`store`: (required) only `EGS` is known to be valid

## Path Parameters

`productId`: self explaining, e.g. `prod-fn` for fortnite

---

_Example Response_

```json
{
  "__typename": "PaginatedOffers",
  "data": [
    {
      "__typename": "OfferError",
      "message": "Error: Failed to get offer purchase"
    }
  ],
  "paging": {
    "count": 1,
    "start": 0,
    "total": 15
  }
}
```
