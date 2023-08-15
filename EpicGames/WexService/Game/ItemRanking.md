## Wex Service - Item Ranking

URL: https://wex-public-service-live-prod.ol.epicgames.com/wex/api/game/v2/item_ratings/:accountId/:templateId \
Method: GET \
Auth Required: Yes (`wexp:profile:{accountId}:commands READ`)

## Path Parameters

`accountId`: Your AccountId <br/>
`templateId`: The Template Id to lookup, e.g. 'Character:Warrior_Starter_Nature_PowerStrike_T03'

---

_Example Response_

```json
{
  "myRating": {
    "gameplayRating": 0,
    "appearanceRating": 0
  },
  "overallRatings": {
    "ratingsKey": "CD.Warrior.Starter.Nature.PowerStrike.T02",
    "discussUrl": "",
    "ratings": [
      {
        "gameplayRating": 11,
        "appearanceRating": 7
      },
      {
        "gameplayRating": 4,
        "appearanceRating": 3
      },
      {
        "gameplayRating": 11,
        "appearanceRating": 13
      },
      {
        "gameplayRating": 15,
        "appearanceRating": 15
      },
      {
        "gameplayRating": 60,
        "appearanceRating": 63
      }
    ]
  }
}
```
