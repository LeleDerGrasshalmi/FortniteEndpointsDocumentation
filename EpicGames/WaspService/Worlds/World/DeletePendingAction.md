## Wasp Service - Delete Pending World Action

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/world/:worldId/pendingActions/action/:actionId \
Method: DELETE \
Auth Required: Yes (`wasp:{namespaceId}:world UPDATE`)

## Path Parameters

`namespaceId`: Check [Readme](../README.md) <br/>
`worldId` The World Id from the [worlds list](./AccountAccessibleWorld.md) or `NewWorld` when validating the name before creating a new world <br/>
`actionId`: Unknown

---

_Example Response (Invalid actionId)_

```json
{
  "errorCode": "errors.com.epicgames.server_error",
  "errorMessage": "Server Error",
  "messageVars": [],
  "numericErrorCode": 1000,
  "originatingService": "wasp-service",
  "intent": "live"
}
```
