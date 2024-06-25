## Wasp Service - Get World Session within Namespace

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/world/:worldId/session \
Method: GET \
Auth Required: Yes (`wasp:{namespaceId}:session READ`)

## Path Parameters

`namespaceId`: Check [Readme](../../README.md) <br/>
`worldId` The World Id from the [worlds list](../AccountAccessibleWorld.md)

---

_Example Response_

```json
{
  "namespaceId": "fn",
  "worldId": "9f5f4fe52d594e0abe3bca3edf62899f",
  "owningSessionId": "a9c000a954e64c328fd925b5953f30b5",
  "sessionKey": "AFD235593B504E6EA9007E1FB5BC8F20",
  "currentPlayers": ["94b1569506b04f9f8557af611e8c5e47"],
  "sessionCreatedAt": "2023-12-08T16:51:31.912Z",
  "lastServerHeartbeat": "2023-12-08T18:48:07.543112137Z",
  "totalSecondsPlayed": null
}
```

_Example Response (no session)_

```json
{
  "messageVars": ["824a1511dd11447b9e5bee7e511f7e84", "fn"],
  "errorMessage": "could not find a session record for world ID '824a1511dd11447b9e5bee7e511f7e84' in namespace 'fn'",
  "errorCode": "errors.com.epicgames.dbs.wasp.world_session_not_found",
  "correlationId": "YjQxMDE0OTljNTJiNDkzYT",
  "numericErrorCode": 1004,
  "responseStatus": 404,
  "intent": "prod",
  "originatingService": "wasp-service"
}
```
