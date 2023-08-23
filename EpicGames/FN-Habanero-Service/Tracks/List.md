## FN - Habanero Service: Tracks List

URL: https://fn-service-habanero-live-public.ogs.live.on.epicgames.com/api/v1/games/:namespace/tracks/query \
Method: GET \
Auth Required: Yes (`rankings:{namespace}:tracks READ`)

## Path Parameters

`namespace`: `fortnite`

# Query Parameters

`endsAfter`: (optional), ISO Date (Start Date of the Data)

---

_Example Response_

```json
[
  {
    "gameId": "fortnite",
    "trackguid": "9d7ebd",
    "rankingType": "ranked-zb",
    "beginTime": "2023-04-01T00:00:00Z",
    "endTime": "2023-10-01T00:00:00Z",
    "divisionCount": 18
  },
  {
    "gameId": "fortnite",
    "trackguid": "2776dc",
    "rankingType": "ranked-br",
    "beginTime": "2023-04-01T00:00:00Z",
    "endTime": "2023-10-01T00:00:00Z",
    "divisionCount": 18
  }
]
```
