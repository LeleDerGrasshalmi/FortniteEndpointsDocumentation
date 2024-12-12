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
    "trackguid": "rrzuel",
    "rankingType": "delmar-competitive",
    "beginTime": "2024-07-23T06:00:00Z",
    "endTime": "2024-10-11T08:00:00Z",
    "divisionCount": 18
  },
  {
    "gameId": "fortnite",
    "trackguid": "S4LT3D",
    "rankingType": "ranked-br",
    "beginTime": "2024-08-16T04:00:01Z",
    "endTime": "2024-11-02T23:59:00Z",
    "divisionCount": 18
  },
  {
    "gameId": "fortnite",
    "trackguid": "P0T4T0",
    "rankingType": "ranked-zb",
    "beginTime": "2024-08-16T04:00:01Z",
    "endTime": "2024-11-02T23:59:00Z",
    "divisionCount": 18
  },
  {
    "gameId": "fortnite",
    "trackguid": "M4rC4S",
    "rankingType": "ranked_blastberry_build",
    "beginTime": "2024-09-24T13:00:00Z",
    "endTime": "2025-01-26T17:59:00Z",
    "divisionCount": 18
  },
  {
    "gameId": "fortnite",
    "trackguid": "L4nC3r",
    "rankingType": "ranked_blastberry_nobuild",
    "beginTime": "2024-09-24T13:00:00Z",
    "endTime": "2025-01-26T17:59:00Z",
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
