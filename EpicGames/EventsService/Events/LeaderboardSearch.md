## Events Service - Event Window Leaderboard Scores

This endpoint is used for retrieving the friends leaderboard in-game.

URL: https://events-public-service-live.ol.epicgames.com/api/v2/games/:gameId/leaderboards/:eventId/:eventWindowId/scores \
Method: POST \
Auth Required: Yes (`{gameId}:profile:{accountId}:commands READ`)

```json
{
  "teams": [["accountId1", "accountId2"], ["accountId3"]]
}
```

## Path Parameters

`gameId`: Fortnite <br/>
`eventId`: from the Event List <br/>
`eventWindowId`: from the Event Windows <br/>

## Query Parameters

`accountId`: Your Account Id <br/>
`fromIndex`: The starting index for the search, e.g., 0 <br/>
`aroundTeamId`: Team Id in the format `accountId1:accountId2:accountId3`. This parameter can be used multiple times <br/>
`findTeams`: boolean, Searches for the entire team if only one account Id is provided (e.g., in a Trio Cup) <br/>

Either `fromIndex` or `aroundTeamId` is required! <br/>
If using `aroundTeamId`, all the `accountId`s of the specified team must be included in the request body! <br/>
Does not work for events before Season 22!

---

_Example Response (shortened)_

```json
[
  {
    "scoreKey": {
      "gameId": "Fortnite",
      "eventId": "epicgames_S34_SoloCashCup_EU",
      "eventWindowId": "S34_SoloCashCup_Event3Round2_EU"
    },
    "teamId": "ddf0172619474ddeb19f855dc065b80c",
    "teamAccountIds": ["ddf0172619474ddeb19f855dc065b80c"],
    "pointsEarned": 352,
    "score": 1548398805990442,
    "rank": 4,
    "percentile": -1,
    "pointBreakdown": {},
    "sessionHistory": [],
    "unscoredSessions": []
  }
]
```
