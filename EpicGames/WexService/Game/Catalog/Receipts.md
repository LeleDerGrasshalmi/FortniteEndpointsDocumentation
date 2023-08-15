## Wex Service - Catalog: Receipts

URL: https://wex-public-service-live-prod.ol.epicgames.com/wex/api/receipts/v1/account/:accountId/receipts \
Method: GET \
Auth Required: Yes (`wexp:profile:{accountId}:receipts READ`)

## Path Parameters

`accountId`: Your AccountId

---

_Example Response (shortened)_

```json
[
  {
    "appStore": "EpicPurchasingService",
    "appStoreId": "d3ec04d33f674fd3a7054b6b6b92d6c9",
    "receiptId": "e2cb0046619e455ca8976c0f280e6387",
    "receiptInfo": "ENTITLEMENT"
  }
]
```
