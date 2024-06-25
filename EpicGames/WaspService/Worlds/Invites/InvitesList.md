## Wasp Service - World Invites

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/invites/world/:worldId \
Method: GET \
Auth Required: Yes (`wasp:{namespaceId}:invite READ`)

## Path Parameters

`namespaceId`: Check [Readme](../../README.md) <br/>
`worldId` The World Id from the [worlds list](../AccountAccessibleWorld.md)

---

_Example Response (no perm)_

```json
{
  "messageVars": ["wasp:fn:invite", "READ"],
  "errorMessage": "Sorry your login does not posses the permissions 'wasp:fn:invite READ' needed to perform the requested operation",
  "errorCode": "errors.com.epicgames.common.missing_permission",
  "correlationId": "ZGI4ZGVlMTBiOTNmNDEyNT",
  "numericErrorCode": 1023,
  "responseStatus": 403,
  "intent": "prod",
  "originatingService": "wasp-service"
}
```
