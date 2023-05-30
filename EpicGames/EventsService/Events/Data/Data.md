## Events Service - Events List (Data)

URL: https://events-public-service-live.ol.epicgames.com/api/v1/events/:gameId/data/:accountId \
Method: GET \
Auth Required: Yes (`{gameId}:profile:{accountId}:commands READ`)

## Path Parameters

`gameId`: Fortnite <br/>
`accountId`: Your Account Id

## Query Parameters

`region`: e.g. EU <br/>
`platform`: e.g. Windows <br/>
`teamAccountIds`: Account Ids seperated by a comma `,`

---

_Example Response (shortened)_

```json
{
  "player": {
    "gameId": "Fortnite",
    "accountId": "94b1569506b04f9f8557af611e8c5e47",
    "tokens": [
      "Arena_S24_Division1",
      "GroupIdentity_GeoIdentity_Germany",
      "GroupIdentity_Lele_is_Cool"
    ],
    "teams": {},
    "pendingPayouts": [],
    "pendingPenalties": {},
    "persistentScores": {
      "Hype_S24_P": 0
    },
    "groupIdentity": {
      "GeoIdentity": "Germany"
    }
  },
  "events": [],
  "templates": [],
  "leaderboardDefs": [],
  "scoringRuleSets": {},
  "payoutTables": {},
  "scores": [],
  "resolvedWindowLocations": {}
}
```
