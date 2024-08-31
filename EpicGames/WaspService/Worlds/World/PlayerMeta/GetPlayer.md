## Wasp Service - Get World Player Meta

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/world/:worldId/playermeta/accountIds/:accountId \
Method: GET \
Auth Required: Yes (`wasp:{namespaceId}:world READ`)

## Path Parameters

`namespaceId`: Check [Readme](../README.md) <br/>
`worldId` The World Id from the [worlds list](./AccountAccessibleWorld.md) <br/>
`accountId`: Target player account id

---

_Example Response (Has Meta)_

```json
{
  "namespaceId": "fn",
  "worldId": "52e1e576226c42ad9563503254f866c1",
  "accountId": "94b1569506b04f9f8557af611e8c5e47",
  "totalSecondsPlayed": 61,
  "lastPlayed": "2024-08-31T10:08:30.134Z",
  "metadata": {}
}
```

_Example Response (No Meta)_

```json
{
  "messageVars": ["fn", "52e1e576226c42ad9563503254f866c1", "dummy"],
  "errorMessage": "could not find playermeta under namespace 'fn', worldID '52e1e576226c42ad9563503254f866c1', for accountId 'dummy'",
  "errorCode": "errors.com.epicgames.dbs.wasp.playermeta_not_found",
  "correlationId": "MjYwNzZiZGI2MzcwNGZkOT",
  "numericErrorCode": 1004,
  "responseStatus": 404,
  "intent": "live",
  "originatingService": "wasp-service"
}
```
