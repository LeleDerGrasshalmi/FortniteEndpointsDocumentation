## Wasp Service - Get Account World Grants

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/grants/world/:worldId/account/:accountId \
Method: GET \
Auth Required: Yes (`wasp:{namespaceId}:grant READ`)

## Path Parameters

`namespaceId`: Check [Readme](../../README.md) <br/>
`worldId` The World Id from the [worlds list](../AccountAccessibleWorld.md) <br/>
`accountId`: The Account Id of the player to check the grants from

---

_Example Response_

```json
[
  {
    "namespaceId": "fn",
    "worldId": "0ad1bf7c2c224b6e9418d3a2c02b5ee7",
    "accountId": "94b1569506b04f9f8557af611e8c5e47",
    "roleId": "world_owner",
    "type": "PERSISTENT",
    "grantedBy": "system",
    "grantedAt": "2023-12-03T16:53:35.63368256Z",
    "expiresAt": "-999999999-01-01T00:00:00+18:00"
  }
]
```
