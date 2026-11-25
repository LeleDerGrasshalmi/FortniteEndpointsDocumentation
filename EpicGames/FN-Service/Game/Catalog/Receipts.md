## FN Service - Receipts

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/game/v2/receipts/:accountId <br/>
Method: GET <br/>
Auth Required: Yes (`fortnite:profile:{accountId}:commands ALL`)

## Path Parameters

`accountId`: Your Account Id

---

*Example Response*

```json
[
  {
    "appStore": "EpicPurchasingService",
    "appStoreId": "0d9a0d1012564f0280ad4ebf3e1e5fce",
    "receiptId": "62f9cfd5447e47bcb09f2260f332cfef",
    "receiptInfo": "ENTITLEMENT"
  }
]
```
