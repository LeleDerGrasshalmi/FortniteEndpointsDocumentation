## Wasp Service - Get World Player Meta (Bulk)

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/world/:worldId/playermeta/bulk/get \
Method: POST \
Auth Required: Yes (`wasp:{namespaceId}:world READ`)

```json
{
  "accountIds": ["epic", "94b1569506b04f9f8557af611e8c5e47"]
}
```

## Path Parameters

`namespaceId`: Check [Readme](../README.md) <br/>
`worldId` The World Id from the [worlds list](./AccountAccessibleWorld.md)

## Parameters

`accountIds`: Account Id's to query the player meta of, must be between 1 and 25 elements

---

_Example Response_

```json
{
  "playermeta": [
    {
      "namespaceId": "fn",
      "worldId": "52e1e576226c42ad9563503254f866c1",
      "accountId": "94b1569506b04f9f8557af611e8c5e47",
      "totalSecondsPlayed": 61,
      "lastPlayed": "2024-08-31T10:08:30.134Z",
      "metadata": {}
    }
  ]
}
```
