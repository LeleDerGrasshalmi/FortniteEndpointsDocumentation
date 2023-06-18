## FN - Habanero Service: Track Info

URL: https://fn-service-habanero-live-public.ogs.live.on.epicgames.com/api/v1/games/:namespace/tracks/:trackguid \
Method: GET \
Auth Required: Yes (`rankings:{namespace}:tracks READ`)

## Path Parameters

`namespace`: `fortnite` <br/>
`trackguid`: The `trackguid` from the Tracks List

---

_Example Response (shortened)_

```json
{
  "gameId": "fortnite",
  "trackguid": "2776dc",
  "rankingType": "ranked-br",
  "beginTime": "2023-04-01T00:00:00Z",
  "endTime": "2023-10-01T00:00:00Z",
  "divisions": [
    {
      "lowerRatingThreshold": 0,
      "upperRatingThreshold": 725,
      "ratingGrace": 0,
      "trackTopPlayers": 0
    },
    {
      "lowerRatingThreshold": 1960,
      "upperRatingThreshold": 2050,
      "ratingGrace": 18,
      "trackTopPlayers": 0
    },
    {
      "lowerRatingThreshold": 2050,
      "upperRatingThreshold": 9999,
      "ratingGrace": 9999,
      "trackTopPlayers": 100000
    }
  ],
  "firstWeekRolloverTime": "2023-04-01T00:00:00Z",
  "leaderboardTrackingEventId": "epicgames_ranked_br_season24"
}
```
