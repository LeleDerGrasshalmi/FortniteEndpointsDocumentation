## Wasp Service - Accessible Worlds within Namespace for Account

URL: https://wasp-service-prod-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/accessibleTo/:accountId \
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
    "world": {
      "namespaceId": "fn",
      "worldId": "79af99dab4164eba8a0e0227c9fc79c9",
      "ownerAccountId": "94b1569506b04f9f8557af611e8c5e47",
      "version": 0,
      "currentVersion": 0,
      "name": "5",
      "createdAt": "2023-12-03T16:03:03.192373371Z",
      "updatedAt": "2023-12-03T16:03:03.200514066Z",
      "sanction": null,
      "metadataConstraint": "juno_default",
      "metadata": {
        "seed": 698
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
    "grants": [],
    "session": null
  },
  {
    "world": {
      "namespaceId": "fn",
      "worldId": "0ad1bf7c2c224b6e9418d3a2c02b5ee7",
      "ownerAccountId": "94b1569506b04f9f8557af611e8c5e47",
      "version": 0,
      "currentVersion": 0,
      "name": "2",
      "createdAt": "2023-12-03T16:53:35.63368256Z",
      "updatedAt": "2023-12-03T16:53:35.644052606Z",
      "sanction": null,
      "metadataConstraint": "juno_default",
      "metadata": {
        "mode": "Sandbox",
        "friendlyCreatures": "On",
        "hostileCreatures": "Off",
        "npcs": "On",
        "dropInventoryOnDeath": "On",
        "seed": 9058374,
        "death": "On",
        "temperature": "Off",
        "thumbnailTableRowName": "Desert_01",
        "staminaDrain": "On",
        "hunger": "Off"
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
    "grants": [],
    "session": null
  }
]
```
