## FN - Habanero Service: Tracks Progress for Account

URL: https://fn-service-habanero-live-public.ogs.live.on.epicgames.com/api/v1/games/:namespace/trackprogress/:accountId \
Method: GET \
Auth Required: Yes (`rankings:{namespace}:playerprogress READ`)

## Path Parameters

`namespace`: `fortnite` <br/>
`accountId`: Can be any Account Id (works for any User, currently even if stats are private)

# Query Parameters

`endsAfter`: (optional), ISO Date (Start Date of the Data)

---

_Example Response_

```json
[
  {
    "gameId": "fortnite",
    "trackguid": "9d7ebd",
    "accountId": "XXXXXXXXXXXXXXXXXXXXX",
    "rankingType": "ranked-zb",
    "lastUpdated": "1970-01-01T00:00:00Z",
    "currentDivision": 0,
    "highestDivision": 0,
    "promotionProgress": 0.0,
    "currentPlayerRanking": null
  },
  {
    "gameId": "fortnite",
    "trackguid": "2776dc",
    "accountId": "XXXXXXXXXXXXXXXXXXXXX",
    "rankingType": "ranked-br",
    "lastUpdated": "2023-05-17T16:08:36.367Z",
    "currentDivision": 3,
    "highestDivision": 3,
    "promotionProgress": 0.19,
    "currentPlayerRanking": null
  }
]
```
