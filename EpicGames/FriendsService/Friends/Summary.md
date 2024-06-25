## Friends Service - Summary

URL: https://friends-public-service-prod.ol.epicgames.com/friends/api/v1/:accountId/summary \
Method: GET \
Auth Required: Yes (`friends:{accountId} READ`)

## Path Parameters

`accountId`: Your Account Id

---

_Example Response_

```json
{
  "friends": [
    {
      "accountId": "94b1569506b04f9f8557af611e8c5e47",
      "groups": [],
      "alias": "lele test",
      "note": "hello from lele's epic api docs",
      "favorite": false,
      "created": "2024-05-10T09:16:39.913Z"
    }
  ],
  "incoming": [
    {
      "accountId": "7b4ec91a76c645edb470dd41d7c6e370",
      "mutual": 3,
      "favorite": false,
      "created": "2024-05-10T11:02:15.625Z"
    }
  ],
  "outgoing": [
    {
      "accountId": "edba7de104fa4069a2bbcc97b7be0c35",
      "mutual": 0,
      "favorite": false,
      "created": "2024-05-10T11:01:47.466Z"
    }
  ],
  "suggested": [],
  "blocklist": [
    {
      "accountId": "5f38c3127c8f44f9b59ae33b095d60b0",
      "created": "2024-05-10T11:03:43.976Z"
    }
  ],
  "settings": {
    "acceptInvites": "public",
    "mutualPrivacy": "ALL"
  },
  "limitsReached": {
    "incoming": false,
    "outgoing": false,
    "accepted": false
  }
}
```
