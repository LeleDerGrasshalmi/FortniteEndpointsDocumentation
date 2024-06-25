## Events Service - Event Window Leaderboard

URL: https://events-public-service-live.ol.epicgames.com/api/v1/leaderboards/:gameId/:eventId/:eventWindowId/:accountId \
Method: GET \
Auth Required: Yes (`{gameId}:profile:{accountId}:commands READ`)

## Path Parameters

`gameId`: Fortnite <br/>
`eventId`: from the Event List <br/>
`eventWindowId`: from the Event Windows <br/>
`accountId`: Your Account Id

## Query Parameters

`page`: 0 (0 - 100) <br/>
`rank`: 1 (The rank is used if page and rank are given (e.g. 54 would still goto page 1 and start at rank 1)) <br/>
`showLiveSessions`: boolean <br/>
`teamAccountIds`: Account Ids seperated by a comma `,` <br/>
`appId`: fortnite

---

_Example Response_

```json
{
  "gameId": "Fortnite",
  "eventId": "epicgames_S24_DuosCashCup_EU",
  "eventWindowId": "S24_DuosCashCup_EU_Event1_Round1",
  "page": 0,
  "totalPages": 0,
  "updatedTime": "2023-05-30T19:13:27.317Z",
  "entries": [],
  "liveSessions": {}
}
```
