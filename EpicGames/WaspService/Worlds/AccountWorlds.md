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
    "worldId": "b29a32d96cb449e7b4bd677f4503d997",
    "ownerAccountId": "94b1569506b04f9f8557af611e8c5e47",
    "version": 0,
    "currentVersion": 0,
    "name": "6",
    "createdAt": "2023-11-12T12:17:25.584193993Z",
    "updatedAt": "2023-11-12T12:17:25.592478165Z",
    "sanction": null,
    "metadataConstraint": "juno_default",
    "metadata": {
      "seed": 818
    },
    "session": {
      "owningSessionId": null,
      "sessionKey": null,
      "currentPlayers": null,
      "sessionCreatedAt": null,
      "lastServerHeartbeat": null,
      "totalSecondsPlayed": 0
    }
  },
  {
    "namespaceId": "fn",
    "worldId": "ed22688b9545447b8c458afb3007d464",
    "ownerAccountId": "94b1569506b04f9f8557af611e8c5e47",
    "version": 0,
    "currentVersion": 0,
    "name": "1",
    "createdAt": "2023-11-10T23:25:52.331111261Z",
    "updatedAt": "2023-11-10T23:25:52.334501405Z",
    "sanction": null,
    "metadataConstraint": "nometadata",
    "metadata": {},
    "session": {
      "owningSessionId": null,
      "sessionKey": null,
      "currentPlayers": null,
      "sessionCreatedAt": null,
      "lastServerHeartbeat": null,
      "totalSecondsPlayed": 0
    }
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
