## Wasp Service - Delete World within Namespace

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/world/:worldId \
Method: DELETE \
Auth Required: Yes (`wasp:{namespaceId}:world DELETE`)

## Path Parameters

`namespaceId`: Check [Readme](../../README.md) <br/>
`worldId` The World Id from the [worlds list](../AccountAccessibleWorld.md)

---

_Example Response_: Status 204

_Example Response (not world owner)_

```json
{
  "messageVars": ["824a1511dd11447b9e5bee7e511f7e84", "fn"],
  "errorMessage": "caller must be the world owner of '824a1511dd11447b9e5bee7e511f7e84':'fn'",
  "errorCode": "errors.com.epicgames.dbs.wasp.world_owner_required",
  "correlationId": "MDA2Yzk4YjVjYzg3NDM3Yj",
  "numericErrorCode": 1003,
  "responseStatus": 403,
  "intent": "prod",
  "originatingService": "wasp-service"
}
```
