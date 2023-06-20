## FN - Habanero Service: Track Progress for Accounts (Bulk)

URL: https://fn-service-habanero-live-public.ogs.live.on.epicgames.com/api/v1/games/:namespace/trackprogress/byAccountIds/:trackguid \
Method: POST \
Auth Required: Yes (`rankings:{namespace}:playerprogress READ`)

```json
{
  "accountIds": ["accountId1", "accountId2"]
}
```

## Path Parameters

`namespace`: `fortnite` <br/>
`trackguid`: The `trackguid` from the Tracks List

## Parameters

`accountIds`: The Account Ids to query (Max 25)

---

_Example Response_

```json
[
  {
    "gameId": "fortnite",
    "trackguid": "2776dc",
    "accountId": "accountId1",
    "rankingType": "ranked-br",
    "lastUpdated": "1970-01-01T00:00:00Z",
    "currentDivision": 0,
    "highestDivision": 0,
    "promotionProgress": 0.0,
    "currentPlayerRanking": null
  },
  {
    "gameId": "fortnite",
    "trackguid": "2776dc",
    "accountId": "94b1569506b04f9f8557af611e8c5e47",
    "rankingType": "ranked-br",
    "lastUpdated": "2023-05-18T21:17:42.603Z",
    "currentDivision": 2,
    "highestDivision": 3,
    "promotionProgress": 0.87,
    "currentPlayerRanking": null
  }
]
```
