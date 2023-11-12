## Wasp Service - Create World within Namespace

URL: https://wasp-service-prod-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/account/:accountId \
Method: POST \
Auth Required: Yes (`wasp:{namespaceId}:world CREATE`)

```json
{
  "metadataConstraint": "juno_default",
  "metadata": {}
}
```

## Path Parameters

`namespaceId`: Check [Readme](../README.md) <br/>
`accountId` Your account Id

## Parameters

`metadataConstraint`: Either `nometadata` or `juno_default` (`juno:default` got deprecated) <br/>
`metadata`: Based on the `metadataConstraint` you need different fields:

- `juno_default`:

  ```json
  {
    "seed": 1
  }
  ```

- `nometadata`: doesnt require any fields, leave the `metadata` object empty

---

_Example Response_

```json
{
  "namespaceId": "fn",
  "worldId": "e49dbfad26014173856bb83ac00cb36b",
  "ownerAccountId": "94b1569506b04f9f8557af611e8c5e47",
  "version": 0,
  "currentVersion": 0,
  "name": "3",
  "createdAt": "2023-11-11T09:55:24.798782065Z",
  "updatedAt": "2023-11-11T09:55:24.807352941Z",
  "sanction": null,
  "metadataConstraint": "juno_default",
  "metadata": {
    "seed": 1
  },
  "session": {
    "owningSessionId": null,
    "sessionKey": null,
    "currentPlayers": null,
    "sessionCreatedAt": null,
    "lastServerHeartbeat": null,
    "totalSecondsPlayed": 0
  }
}
```

_Example Response (world limit reached)_

```json
{
  "messageVars": ["8", "fn"],
  "errorMessage": "This account has already created the maximum number of worlds (8) in namespace 'fn'",
  "errorCode": "errors.com.epicgames.dbs.wasp.world_limit_reached",
  "correlationId": "YmMxYzhjMTYwZDcwNDY4Nz",
  "numericErrorCode": 1004,
  "responseStatus": 400,
  "intent": "prod",
  "originatingService": "wasp-service"
}
```
