## Wasp Service - Get World within Namespace

URL: https://wasp-service-prod-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/world/:worldId \
Method: GET \
Auth Required: Yes (`wasp:{namespaceId}:world READ`)

## Path Parameters

`namespaceId`: Check [Readme](../README.md) <br/>
`worldId` The World Id from the [worlds list](./AccountWorlds.md)

---

_Example Response_

```json
{
  "namespaceId": "fn",
  "worldId": "d4bf6ca6b65a497b94ad5225a40624b6",
  "ownerAccountId": "94b1569506b04f9f8557af611e8c5e47",
  "version": 0,
  "currentVersion": 0,
  "name": "7",
  "createdAt": "2023-11-11T09:58:25.215958467Z",
  "updatedAt": "2023-11-12T12:41:41.065177278Z",
  "sanction": null,
  "metadataConstraint": "juno_default",
  "metadata": {
    "seed": 72
  },
  "session": null
}
```

_Example Response (no world permissions)_

```json
{
  "messageVars": [
    "94b1569506b04f9f8557af611e8c5e47",
    "world:keyholder",
    "fn",
    "824a1511dd11447b9e5bee7e511f7e84"
  ],
  "errorMessage": "account '94b1569506b04f9f8557af611e8c5e47' does not have permission 'world:keyholder' in namespace 'fn' for world '824a1511dd11447b9e5bee7e511f7e84'",
  "errorCode": "errors.com.epicgames.dbs.wasp.permission_not_allowed",
  "correlationId": "ZjBlMzBhMDkzOWU2NDE5Nz",
  "numericErrorCode": 1003,
  "responseStatus": 403,
  "intent": "prod",
  "originatingService": "wasp-service"
}
```
