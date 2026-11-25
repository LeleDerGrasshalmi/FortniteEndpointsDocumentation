## Wasp Service - Create Worlds Grant

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/grants/world/:worldId <br/>
Method: POST <br/>
Auth Required: Yes (`wasp:{namespaceId}:grant CREATE`)

## Path Parameters

`namespaceId`: Check [Readme](../../README.md) <br/>
`worldId`: The World Id from the [worlds list](../AccountAccessibleWorld.md)

---

*Example Response*

Currently you always get this error, unrelated to your namespaceId, worldId or _anything_ else.

```json
{
  "messageVars": [],
  "errorMessage": "Unauthorized",
  "errorCode": "errors.com.epicgames.unauthorized",
  "correlationId": "NDBhODY0NTlkODNkNDBkNT",
  "numericErrorCode": 1002,
  "responseStatus": 401,
  "intent": "prod",
  "originatingService": "wasp-service"
}
```
