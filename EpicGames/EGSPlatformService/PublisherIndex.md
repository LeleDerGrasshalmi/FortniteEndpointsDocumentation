## EGS Platform Service - Publisher Index

URL: https://egs-platform-service.store.epicgames.com/api/v1/egs/publisher-index \
Method: GET \
Auth Required: No

## Query Parameters

`count`: (required) 1 <= 100 <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`start`: (required) start index <br/>
`storeId`: (required) valid Catalog Service Stores, e.g. `EGS`

---

_Example Response_

```json
{
  "__typename": "PaginatedPublisherIndex",
  "data": [
    {
      "contact": {
        "addressLine1": null,
        "addressLine2": null,
        "city": "Lochau",
        "country": "Austria",
        "email": "anqa.game@gmail.com",
        "phoneNumber": null,
        "postalCode": null,
        "stateProvince": null
      },
      "offers": [
        {
          "id": "ef05c59d9d8445859fda90a5d7f1991a",
          "namespace": "c0d21f55048943b990644fa9f43322cb",
          "title": "Djinn - The Forbidden Knowledge"
        }
      ],
      "sellerId": "o-bmj8klvfef59yguur3ejdj5zpd2zlg",
      "sellerName": "Anqa Game e.U."
    },
    {
      "contact": null,
      "offers": [
        {
          "id": "9c15cd76b66a4b98b0dbb2b61d2ff40d",
          "namespace": "68f79f57d943452a93f56b6ef66aa76c",
          "title": "Zoria Age of Shattering"
        },
        {
          "id": "a7e871c5b9c04c25aa0491924e571334",
          "namespace": "024b587ece4b44248759adaacb77a5d4",
          "title": "Liberte"
        },
        {
          "id": "61d13d6fe0c84016a8bacd6fa14cab0e",
          "namespace": "b8abdf9f9bc64ed6b4128a71fd47607f",
          "title": "Gamedec"
        }
      ],
      "sellerId": "o-9z65aawjyvtc2yfpv8ud48hjx6xhv9",
      "sellerName": "Anshar Publishing"
    }
  ],
  "paging": {
    "count": 2,
    "start": 99,
    "total": 1785
  }
}
```
