## FN - Habanero Service: Track Progress for Accounts by Ranking Type (Bulk)

URL: https://fn-service-habanero-live-public.ogs.live.on.epicgames.com/api/v1/games/:namespace/trackprogress/bulkByRankingType \
Method: POST \
Auth Required: Yes (`rankings:{namespace}:playerprogress READ`)

```json
{
  "accountIds": ["accountId1", "accountId2"]
}
```

## Path Parameters

`namespace`: `fortnite`

## Parameters

`accountIds`: The Account Ids to query (Max 25)

## Query Parameters

`rankingType`: (required) The tracks ranking type, ex. `ranked-br` <br/>
`endsAfter`: (optional), ISO Date (Start Date of the Data)

---

_Example Response_

```json
[
  {
    "gameId": "fortnite",
    "trackguid": "c0off3",
    "accountId": "94b1569506b04f9f8557af611e8c5e47",
    "rankingType": "ranked-br",
    "lastUpdated": "1970-01-01T00:00:00Z",
    "currentDivision": 0,
    "highestDivision": 0,
    "promotionProgress": 0.0,
    "currentPlayerRanking": null
  },
  {
    "gameId": "fortnite",
    "trackguid": "c0off3",
    "accountId": "5f38c3127c8f44f9b59ae33b095d60b0",
    "rankingType": "ranked-br",
    "lastUpdated": "1970-01-01T00:00:00Z",
    "currentDivision": 0,
    "highestDivision": 0,
    "promotionProgress": 0.0,
    "currentPlayerRanking": null
  }
]
```
