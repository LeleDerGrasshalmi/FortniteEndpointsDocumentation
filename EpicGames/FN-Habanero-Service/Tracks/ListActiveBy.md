## FN - Habanero Service: Tracks List (Active by Date)

URL: https://fn-service-habanero-live-public.ogs.live.on.epicgames.com/api/v1/games/fortnite/tracks/activeBy/:startDate \
Method: GET \
Auth Required: Yes (`rankings:{namespace}:tracks READ`)

## Path Parameters

`namespace`: `fortnite` <br/>
`startDate`: Specify the date which tracks should be active, and only return those (ISO Date)

---

_Example Response_

```json
[
  {
    "gameId": "fortnite",
    "trackguid": "gr4p3s",
    "rankingType": "delmar-competitive",
    "beginTime": "2026-03-19T06:00:01Z",
    "endTime": "2026-07-01T00:00:00Z",
    "divisionCount": 18,
    "leaderboardTrackingEventId": "epicgames_ranked_rr_season11"
  },
  {
    "gameId": "fortnite",
    "trackguid": "L3AGUE",
    "rankingType": "ranked-br-combined",
    "beginTime": "2026-03-19T06:00:01Z",
    "endTime": "2026-07-01T23:59:00Z",
    "divisionCount": 18,
    "leaderboardTrackingEventId": "epicgames_ranked_br_season40"
  },
  {
    "gameId": "fortnite",
    "trackguid": "c1ty17",
    "rankingType": "ranked-feral",
    "beginTime": "2026-03-19T06:00:01Z",
    "endTime": "2026-07-01T23:59:00Z",
    "divisionCount": 18,
    "leaderboardTrackingEventId": "epicgames_ranked_feral_season40"
  },
  {
    "gameId": "fortnite",
    "trackguid": "ST33L5",
    "rankingType": "ranked_blastberry_build",
    "beginTime": "2026-02-19T09:00:01Z",
    "endTime": "2026-08-18T23:59:00Z",
    "divisionCount": 18,
    "leaderboardTrackingEventId": "epicgames_ranked_blastberry_build_season39v2"
  },
  {
    "gameId": "fortnite",
    "trackguid": "ST0RM5",
    "rankingType": "ranked_blastberry_nobuild",
    "beginTime": "2026-02-19T09:00:01Z",
    "endTime": "2026-08-18T23:59:00Z",
    "divisionCount": 18,
    "leaderboardTrackingEventId": "epicgames_ranked_blastberry_zb_season39v2"
  }
]
```
