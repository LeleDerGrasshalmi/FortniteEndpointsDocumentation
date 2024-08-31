## Wasp Service - Update World within Namespace

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/world/:worldId \
Method: PUT \
Auth Required: Yes (`wasp:{namespaceId}:world UPDATE`)

```json
{
  "metadata": {
    "recruitedCreaturePermaDeath": "On"
  },
  "customName": "my new name"
}
```

## Path Parameters

`namespaceId`: Check [Readme](../README.md) <br/>
`worldId` The World Id from the [worlds list](./AccountAccessibleWorld.md)

## Parameters

`metadata`: Based on the `metadataConstraint` you need different fields, this are the same metadata fields from the [world creation](./WorldInfo.md), but most props wont be modifiable <br/>
`customName`: The new custom world name

---

_Example Response_

```json
{
  "namespaceId": "fn",
  "worldId": "52e1e576226c42ad9563503254f866c1",
  "ownerAccountId": "94b1569506b04f9f8557af611e8c5e47",
  "version": 0,
  "currentVersion": 0,
  "name": "5",
  "customName": "my custom name",
  "customNameChangeAllowedAt": "2024-08-31T10:26:32.394266599Z",
  "createdAt": "2024-05-07T17:13:58.250022091Z",
  "updatedAt": "2024-05-07T17:17:52.993752952Z",
  "sanction": null,
  "metadataConstraint": "nometadata",
  "metadata": {},
  "session": {
    "owningSessionId": null,
    "sessionKey": null,
    "currentPlayers": null,
    "sessionCreatedAt": null,
    "lastServerHeartbeat": "2024-08-31T10:08:45.556731589Z",
    "totalSecondsPlayed": 215
  },
  "pendingActions": []
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
