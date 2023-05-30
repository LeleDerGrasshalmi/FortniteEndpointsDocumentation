## Events Service - Events List (Download)

URL: https://events-public-service-live.ol.epicgames.com/api/v1/events/:gameId/download/:accountId \
Method: GET \
Auth Required: Yes (`{gameId}:profile:{accountId}:commands READ`)

## Path Parameters

`gameId`: Fortnite <br/>
`accountId`: Your Account Id

## Query Parameters

`region`: e.g. EU (if not specified shows for all regions!) <br/>
`showPastEvents`: true <br/>
`showPrivateEvents`: boolean, throws because you dont have access

---

_Example Response (shortened)_

```json
{
  "events": [],
  "templates": [],
  "leaderboardDefs": [],
  "scoringRuleSets": {},
  "scoreLocationPayoutTables": {},
  "payoutTables": {},
  "resolvedWindowLocations": {}
}
```
