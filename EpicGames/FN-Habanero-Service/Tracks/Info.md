## FN - Habanero Service: Track Info

URL: https://fn-service-habanero-live-public.ogs.live.on.epicgames.com/api/v1/games/:namespace/tracks/byGUID/:trackguid \
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
  "endTime": "2023-06-20T08:00:00Z",
  "divisionCount": 18
}
```
