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
    "trackguid": "rrhr6d",
    "rankingType": "delmar-competitive",
    "beginTime": "2024-12-01T05:00:00Z",
    "endTime": "2025-02-21T08:00:00Z",
    "divisionCount": 18
  },
  {
    "gameId": "fortnite",
    "trackguid": "DR3AM5",
    "rankingType": "ranked-figment-nobuild",
    "beginTime": "2024-12-16T14:00:00Z",
    "endTime": "2025-02-21T23:59:00Z",
    "divisionCount": 18
  },
  {
    "gameId": "fortnite",
    "trackguid": "P3PP3R",
    "rankingType": "ranked_blastberry_build",
    "beginTime": "2024-11-02T06:00:01Z",
    "endTime": "2025-02-21T23:59:00Z",
    "divisionCount": 18
  },
  {
    "gameId": "fortnite",
    "trackguid": "SP1D3R",
    "rankingType": "ranked-zb",
    "beginTime": "2024-12-01T06:00:06Z",
    "endTime": "2025-02-21T23:59:00Z",
    "divisionCount": 18
  },
  {
    "gameId": "fortnite",
    "trackguid": "Gl4ss1",
    "rankingType": "ranked-br",
    "beginTime": "2024-12-01T06:00:06Z",
    "endTime": "2025-02-21T23:59:00Z",
    "divisionCount": 18
  },
  {
    "gameId": "fortnite",
    "trackguid": "W4FFL3",
    "rankingType": "ranked_blastberry_nobuild",
    "beginTime": "2024-11-02T06:00:01Z",
    "endTime": "2025-02-21T23:59:00Z",
    "divisionCount": 18
  },
  {
    "gameId": "fortnite",
    "trackguid": "M3M0RY",
    "rankingType": "ranked-figment-build",
    "beginTime": "2024-12-16T14:00:00Z",
    "endTime": "2025-02-21T23:59:00Z",
    "divisionCount": 18
  },
  {
    "gameId": "fortnite",
    "trackguid": "G4RL1C",
    "rankingType": "ranked-feral",
    "beginTime": "2024-12-11T14:00:00Z",
    "endTime": "2025-02-21T23:59:00Z",
    "divisionCount": 18
  }
]
```
