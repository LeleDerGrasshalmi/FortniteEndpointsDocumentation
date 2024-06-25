## Friends Service - Friends List (Old)

URL: https://friends-public-service-prod.ol.epicgames.com/friends/api/public/friends/:accountId \
Method: GET \
Auth Required: Yes (`friends:{accountId} READ`)

## Path Parameters

`accountId`: Your Account Id

---

_Example Response_

```json
[
  {
    "accountId": "94b1569506b04f9f8557af611e8c5e47",
    "status": "ACCEPTED",
    "direction": "INBOUND",
    "alias": "lele test",
    "note": "hello from lele's epic api docs",
    "created": "2024-05-10T09:16:39.913Z",
    "favorite": false
  },
  {
    "accountId": "e66a9759664a416bb1bbb7ab28b3fae9",
    "status": "ACCEPTED",
    "direction": "INBOUND",
    "created": "2022-10-10T18:46:42.000Z",
    "favorite": false
  },
  {
    "accountId": "edba7de104fa4069a2bbcc97b7be0c35",
    "status": "ACCEPTED",
    "direction": "OUTBOUND",
    "note": "Mr. API",
    "created": "2022-11-19T22:15:22.000Z",
    "favorite": false
  }
]
```
