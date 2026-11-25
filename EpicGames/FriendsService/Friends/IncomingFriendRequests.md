## Friends Service - Incoming Friend Requests (sent by others)

URL: https://friends-public-service-prod.ol.epicgames.com/friends/api/v1/:accountId/incoming <br/>
Method: GET <br/>
Auth Required: Yes (`friends:{accountId} READ`)

## Path Parameters

`accountId`: Your Account Id

---

*Example Response*

```json
[
  {
    "accountId": "7b4ec91a76c645edb470dd41d7c6e370",
    "groups": [],
    "alias": "",
    "note": "",
    "favorite": false,
    "created": "2024-05-10T11:02:15.625Z"
  }
]
```
