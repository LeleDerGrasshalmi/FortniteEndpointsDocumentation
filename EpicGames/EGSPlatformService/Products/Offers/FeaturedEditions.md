## EGS Platform Service - Product Featured Editions

URL: https://egs-platform-service.store.epicgames.com/api/v1/egs/products/:productId/featured-offers/editions \
Method: GET \
Auth Required: No

## Query Parameters

`count`: (required) element count to return <br/>
`country`: (required) ISO 3166 - Alpha 2 Code <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`start`: (required) start index <br/>
`store`: (required) valid Catalog Service Stores, e.g. `EGS`

## Path Parameters

`productId`: self explaining, e.g. `prod-fn` for fortnite

---

_Example Response_

```json
{
  "__typename": "PaginatedOffers",
  "data": [],
  "paging": {
    "count": 0,
    "start": 0,
    "total": 0
  }
}
```
