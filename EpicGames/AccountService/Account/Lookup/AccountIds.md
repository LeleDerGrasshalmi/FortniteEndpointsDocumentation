## Account Service - Lookup by Account Ids

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account \
Method: GET \
Auth Required: Yes (No Permission required)

## Query Parameters

`accountId`: Accound Ids, either use the query multiple times or seperate the Ids by a `,` Comma **[Max 100 per Request]**

---

_Example Response_

```json
[
  {
    "id": "020b5d9042174a7692f20db8e23b84d1",
    "displayName": "nintendo test ac",
    "externalAuths": {
      "nintendo": {
        "accountId": "020b5d9042174a7692f20db8e23b84d1",
        "type": "nintendo",
        "externalAuthIdType": "nintendo_id",
        "authIds": []
      }
    }
  },
  {
    "id": "94b1569506b04f9f8557af611e8c5e47",
    "displayName": "lele stw moment",
    "externalAuths": {}
  }
]
```
