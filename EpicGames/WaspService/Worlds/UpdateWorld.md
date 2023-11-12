## Wasp Service - Update World within Namespace

URL: https://wasp-service-prod-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/world/:worldId \
Method: PUT \
Auth Required: Yes (`wasp:{namespaceId}:world UPDATE`)

```json
{
  "metadata": {
    "seed": 72
  }
}
```

## Path Parameters

`namespaceId`: Check [Readme](../README.md) <br/>
`worldId` The World Id from the [worlds list](./AccountWorlds.md)

## Parameters

`metadata`: Based on the `metadataConstraint` you need different fields, this are the same metadata fields from the [world creation](./WorldInfo.md)

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
  "updatedAt": "2023-11-12T12:35:30.781087513Z",
  "sanction": null,
  "metadataConstraint": "juno_default",
  "metadata": {
    "seed": 72
  },
  "session": null
}
```

_Example Response (not world owner)_

```json
{
  "messageVars": ["824a1511dd11447b9e5bee7e511f7e84", "fn"],
  "errorMessage": "caller must be the world owner of '824a1511dd11447b9e5bee7e511f7e84':'fn'",
  "errorCode": "errors.com.epicgames.dbs.wasp.world_owner_required",
  "correlationId": "NzM2MjBmNGNjMDZlNDVkZT",
  "numericErrorCode": 1003,
  "responseStatus": 403,
  "intent": "prod",
  "originatingService": "wasp-service"
}
```
