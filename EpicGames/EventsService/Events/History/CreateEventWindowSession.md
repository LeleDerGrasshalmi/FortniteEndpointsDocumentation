## Events Service - Add Event Window Session Result

URL: https://events-public-service-live.ol.epicgames.com/api/v1/events/:gameId/:eventId/:eventWindowId/history \
Method: POST \
Auth Required: Yes (`{gameId}:matchmaking:session UPDATE`)

```json
{
  "teamAccountIds": ["94b1569506b04f9f8557af611e8c5e47"],
  "sessionSummary": {
    "sessionId": "227a1e5823ae4c108ec4c32c3bb3884a",
    "endTime": "2022-12-17T22:41:15.323Z",
    "trackedStats": {}
  }
}
```

## Parameters

`gameId`: Fortnite <br/>
`eventId`: e.g. epicgames_S23_Lettuce (Mr Beast Extreme Challenge) <br/>
`eventWindowId`: e.g. S23_Lettuce (Mr Beast Extreme Challenge Window)

> Examples for **trackedStats**

Mr Beast Extreme Challenge:

```json
{
  "CREATIVE_COLLECT_ITEMS_STAT": 98,
  "CREATIVE_SCORE_STAT": 88214,
  "PLACEMENT_STAT_INDEX": 1,
  "TIME_ALIVE_STAT": 926
}
```

Arena:

```json
{
  "PLACEMENT_STAT_INDEX": 50,
  "TIME_ALIVE_STAT": 0,
  "TEAM_ELIMS_STAT_INDEX": 0,
  "PLACEMENT_TIEBREAKER_STAT": 50,
  "VICTORY_ROYALE_STAT": 0
}
```

Late Game Arena (Creative):

```json
{
  "CREATIVE_SCORE_STAT": 0,
  "TEAM_ELIMS_STAT_INDEX": 4,
  "CREATIVE_LAP_TIME_STAT": 0,
  "MATCH_PLAYED_STAT": 1,
  "CREATIVE_ROUNDWINS_STAT": 0,
  "CREATIVE_TIME_ALIVE_STAT": 239427,
  "CREATIVE_AI_ELIMINATIONS_STAT": 0,
  "CREATIVE_OBJECTIVES_STAT": 0,
  "VICTORY_ROYALE_STAT": 0,
  "CREATIVE_COLLECT_ITEMS_STAT": 0,
  "CREATIVE_SPAWNS_LEFT_STAT": 0,
  "CREATIVE_REMAINING_HEALTH_STAT": 0,
  "CREATIVE_ELIMINATED_STAT": 3,
  "CREATIVE_ASSISTS_STAT": 10,
  "PLACEMENT_STAT_INDEX": 6,
  "TIME_ALIVE_STAT": 239,
  "CREATIVE_ELIMINATIONS_STAT": 4,
  "CREATIVE_TIME_STAT": 0,
  "CREATIVE_DAMAGE_TAKEN_STAT": 1110,
  "PLACEMENT_TIEBREAKER_STAT": 15,
  "CREATIVE_DAMAGE_DEALT_STAT": 2044
}
```
