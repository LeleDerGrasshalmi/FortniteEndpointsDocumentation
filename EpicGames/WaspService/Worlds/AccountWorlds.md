## Wasp Service - Account Worlds within Namespace

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/ownedBy/:accountId \
Method: GET \
Auth Required: Yes (`wasp:{namespaceId}:world READ`)

## Path Parameters

`namespaceId`: Check [Readme](../README.md) <br/>
`accountId` Your account Id

---

_Example Response_

```json
[
  {
    "namespaceId": "fn",
    "worldId": "17abf5d94fd74b9383f4cf3a05bf2472",
    "ownerAccountId": "94b1569506b04f9f8557af611e8c5e47",
    "version": 0,
    "currentVersion": 0,
    "name": "3",
    "customName": "finalyl",
    "customNameChangeAllowedAt": "2024-08-31T10:10:15.70652891Z",
    "createdAt": "2023-12-08T22:11:21.621143112Z",
    "updatedAt": "2024-05-09T09:17:11.816934562Z",
    "sanction": null,
    "metadataConstraint": "juno_default",
    "metadata": {
      "mode": "Survival",
      "friendlyCreatures": "On",
      "hostileCreatures": "On",
      "npcs": "Off",
      "dropInventoryOnDeath": "Off",
      "seed": 18937492,
      "death": "On",
      "temperature": "On",
      "thumbnailTableRowName": "test",
      "staminaDrain": "On",
      "hunger": "On",
      "devSettings": "[]"
    },
    "session": null,
    "pendingActions": []
  },
  {
    "namespaceId": "fn",
    "worldId": "52e1e576226c42ad9563503254f866c1",
    "ownerAccountId": "94b1569506b04f9f8557af611e8c5e47",
    "version": 0,
    "currentVersion": 0,
    "name": "5",
    "customName": null,
    "customNameChangeAllowedAt": null,
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
]
```

_Example Response (different account)_

```json
{
  "messageVars": ["94b1569506b04f9f8557af611e8c5e47", "hi_github"],
  "errorMessage": "caller is '94b1569506b04f9f8557af611e8c5e47', but tried to perform an operation reserved for accountId 'hi_github'",
  "errorCode": "errors.com.epicgames.dbs.wasp.account_mismatch",
  "correlationId": "MzQwNDE3YzFjZWYzNDU5NW",
  "numericErrorCode": 1003,
  "responseStatus": 403,
  "intent": "prod",
  "originatingService": "wasp-service"
}
```
