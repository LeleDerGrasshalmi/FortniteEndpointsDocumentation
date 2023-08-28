## Library Service - All Playtime

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/playtime/account/:accountId/all \
Method: GET \
Auth Required: Yes (`library:public:{accountId}:playtime:all READ`)

## Path Parameters

`accountId`: Your Account Id

---

_Example Response_

```json
[
  {
    "accountId": "94b1569506b04f9f8557af611e8c5e47",
    "artifactId": "Fortnite",
    "totalTime": 68363
  },
  {
    "accountId": "94b1569506b04f9f8557af611e8c5e47",
    "artifactId": "UnrealTournamentEditor",
    "totalTime": 8669
  },
  {
    "accountId": "94b1569506b04f9f8557af611e8c5e47",
    "artifactId": "WorldExplorersLive",
    "totalTime": 1407
  }
]
```
