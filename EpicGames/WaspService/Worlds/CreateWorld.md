## Wasp Service - Create World within Namespace

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/account/:accountId \
Method: POST \
Auth Required: Yes (`wasp:{namespaceId}:world CREATE`)

```json
{
  "namespaceId": "",
  "worldId": "77455b75-464a-8f68-60dc-0ea9327b2306",
  "ownerAccountId": "94b1569506b04f9f8557af611e8c5e47",
  "name": "",
  "customName": "hello github - whats up",
  "sanction": {
    "worldLocked": false,
    "worldOwnerFix": false,
    "multiplayerRestrictions": false,
    "checkpointId": "",
    "coordinates": ""
  },
  "version": 0,
  "metadataConstraint": "juno_default",
  "metadata": {
    "seed": 40928926,
    "mode": "Cozy",
    "hostileCreatures": "On",
    "friendlyCreatures": "On",
    "dropInventoryOnDeath": "Off",
    "hunger": "Off",
    "staminaDrain": "Off",
    "npcs": "On",
    "thumbnailTableRowName": "Night_01",
    "temperature": "Off",
    "death": "On",
    "friendlyFire": "Off",
    "powerSystem": "Off",
    "recruitedCreaturePermaDeath": "Off",
    "difficulty": "Easy",
    "eliteHostileCreatures": "Off",
    "flying": "Off"
  },
  "session": {
    "namespaceId": "",
    "worldId": "",
    "owningSessionId": "",
    "sessionKey": "",
    "currentPlayers": [],
    "totalSecondsPlayed": 0
  },
  "pendingActions": []
}
```

## Path Parameters

`namespaceId`: Check [Readme](../README.md) <br/>
`accountId` Your account Id

## Parameters

There are many parameters that may seem useless, however the client sends them, so they are documented here. <br/>
The example payload is a real world payload sent by the client on v31.00.

`namespaceId`: Leave as an empty string, its ignored by the server <br/>
`worldId`: A UUIDv4, its ignored by the server <br/>
`ownerAccountId`: Your Account Id, its ignored by the server <br/>
`name`: Leave as an empty string, its ignored by the server <br/>
`customName`: Custom world display name <br/>
`sanction`: Leave like the example, its ignored by the server <br/>
`session`: Leave like the example, its ignored by the server <br/>
`version`: Leave as 0, its ignored by the server <br/>
`pendingActions`: Leave as empty array, its ignored by the server <br/>
`metadataConstraint`: Either `nometadata` or `juno_default` (`juno:default` got deprecated) <br/>
`metadata`: Based on the `metadataConstraint` you need different fields:

- `juno_default`:

  ```json
  {
    "seed": 9058374,
    "mode": "Sandbox",
    "hostileCreatures": "Off",
    "friendlyCreatures": "On",
    "dropInventoryOnDeath": "On",
    "hunger": "Off",
    "staminaDrain": "On",
    "npcs": "On",
    "thumbnailTableRowName": "Desert_01",
    "temperature": "Off",
    "death": "On"
  }
  ```

  These boolean like values can be `On` or `Off`.
  The `mode` can be `Survival` or `Sandbox`.

- `nometadata`: Requires that the `metadata` is empty

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
