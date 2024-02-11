## FN - Habanero Service: Tracks List

URL: https://fn-service-habanero-live-public.ogs.live.on.epicgames.com/api/v1/games/:namespace/tracks/query \
Method: GET \
Auth Required: Yes (`rankings:{namespace}:tracks READ`)

## Path Parameters

`namespace`: `fortnite`

# Query Parameters

`endsAfter`: (optional), ISO Date (Filteres that the tracks end after that date) <br/>
`rankingType`: (optional) only include a certain ranking type, see [info](../README.md) for possible values

---

_Example Response_

```json
[
  {
    "gameId": "fortnite",
    "trackguid": "dmd372",
    "rankingType": "delmar-competitive",
    "beginTime": "2023-12-07T00:00:18Z",
    "endTime": "2025-01-01T07:00:17Z",
    "divisionCount": 18
  },
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
