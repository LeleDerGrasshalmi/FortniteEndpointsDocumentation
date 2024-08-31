## Wasp Service - Get World within Namespace

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/world/:worldId \
Method: GET \
Auth Required: Yes (`wasp:{namespaceId}:world READ`)

## Path Parameters

`namespaceId`: Check [Readme](../README.md) <br/>
`worldId` The World Id from the [worlds list](./AccountAccessibleWorld.md)

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
