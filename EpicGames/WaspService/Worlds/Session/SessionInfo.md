## Wasp Service - Get World Session within Namespace

URL: https://wasp-service-prod-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/world/:worldId/session \
Method: GET \
Auth Required: Yes (`wasp:{namespaceId}:session READ`)

## Path Parameters

`namespaceId`: Check [Readme](../../README.md) <br/>
`worldId` The World Id from the [worlds list](../AccountWorlds.md)

---

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
