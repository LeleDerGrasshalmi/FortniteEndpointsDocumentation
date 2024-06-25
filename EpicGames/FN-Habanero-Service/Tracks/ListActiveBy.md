## FN - Habanero Service: Tracks List (Active by Date)

URL: https://fn-service-habanero-live-public.ogs.live.on.epicgames.com/api/v1/games/fortnite/tracks/activeBy/:startDate \
Method: GET \
Auth Required: Yes (`rankings:{namespace}:tracks READ`)

## Path Parameters

`namespace`: `fortnite` <br/>
`startDate`: Specify the date which tracks should be active, and only return those

---

_Example Response_

```json
[
  {
    "gameId": "fortnite",
    "trackguid": "EYpme7",
    "rankingType": "ranked-br",
    "beginTime": "2023-12-03T08:00:18Z",
    "endTime": "2025-01-01T07:00:17Z",
    "divisionCount": 18
  },
  {
    "gameId": "fortnite",
    "trackguid": "d0zEcd",
    "rankingType": "ranked-zb",
    "beginTime": "2023-12-03T08:00:18Z",
    "endTime": "2025-01-01T07:00:17Z",
    "divisionCount": 18
  }
]
```
