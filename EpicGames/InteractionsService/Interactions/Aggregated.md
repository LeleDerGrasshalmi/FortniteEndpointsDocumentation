## Interactions Service - Aggregated

URL: https://interactions-service-prod.ol.epicgames.com/api/v2/interactions/aggregated/:namespace/:accountId \
Method: GET  \
Auth Required: Yes (`interactions:{namespace}:{accountId} READ`)

## Path Parameters
`accountId`: Your AccountId
`namespace`: e.g. `Fortnite`

## Query Parameters
`limit`: (Optional) Max 200 per request  
`preferredInteractionType`: (Optional) Filter preferred interaction type (e.g. `FriendshipDelete`, `FriendshipAcceptReceived` or `PartyJoined`)

---

### Example Response: Status 200

```json
{
  "aggregatedInteractions": [
    {
      "fromAccountId": "192b217e425b429f8b52c2004dbbaa85",
      "toAccountId": "192b217e425b429f8b52c2004dbbaa85",
      "latestInteraction": {
        "interactionType": "FriendshipDelete",
        "happenedAt": 1761437841841
      },
      "interactionScore": {
        "total": 0,
        "count": 0
      },
      "interactionCount": 0
    },
    {
      "fromAccountId": "192b217e425b429f8b52c2004dbbaa85",
      "toAccountId": "511f1fb7f45749e5b332891243930cf5",
      "latestInteraction": {
        "interactionType": "GamePlayed",
        "happenedAt": 1772311097000,
        "app": "Chapter_7__Season_1"
      },
      "interactionScore": {
        "total": 412,
        "count": 916
      },
      "interactionCount": 916
    }
  ]
}
```