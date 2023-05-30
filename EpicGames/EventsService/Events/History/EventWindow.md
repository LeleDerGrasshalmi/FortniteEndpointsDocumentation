## Events Service - My Event Window History

URL: https://events-public-service-live.ol.epicgames.com/api/v1/events/:gameId/:eventId/:eventWindowId/history/:accountId \
Method: GET \
Auth Required: Yes (`{gameId}:profile:{accountId}:commands READ`)

## Path Parameters

`gameId`: Fortnite <br/>
`eventId`: e.g. epicgames_S23_Lettuce (Mr Beast Extreme Challenge) <br/>
`eventWindowId`: e.g. S23_Lettuce (Mr Beast Extreme Challenge Window)

_Example Response_

```json
[
  {
    "scoreKey": {
      "gameId": "Fortnite",
      "eventId": "epicgames_S24_DuosCashCup_EU",
      "eventWindowId": "S24_DuosCashCup_EU_Event1_Round1",
      "_scoreId": null
    },
    "teamId": "94b1569506b04f9f8557af611e8c5e47",
    "teamAccountIds": ["94b1569506b04f9f8557af611e8c5e47"],
    "liveSessionId": null,
    "pointsEarned": 944,
    "score": 944.0,
    "rank": 279737,
    "percentile": 0.12,
    "pointBreakdown": {
      "PLACEMENT_STAT_INDEX:14": {
        "timesAchieved": 7,
        "pointsEarned": 14
      }
    },
    "sessionHistory": [
      {
        "sessionId": "ccd6b89095b14836873bde658c3fcc1f",
        "endTime": "2023-05-18T21:17:42.614Z",
        "trackedStats": {
          "PLACEMENT_STAT_INDEX": 1
        }
      }
    ],
    "unscoredSessions": []
  }
]
```
