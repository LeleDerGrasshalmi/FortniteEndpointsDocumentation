## Wex Service - Search Friends

URL: https://wex-public-service-live-prod.ol.epicgames.com/wex/api/game/v2/friends/:accountId/search \
Method: GET \
Auth Required: Yes (`wexp:profile:{accountId}:commands READ`)

## Path Parameters

`accountId`: Your AccountId

## Query Parameters

`name`: DisplayName to search for

---

_Example Response (shortened)_

```json
[
  {
    "accountId": "99201479009a4ab7b0bbdf3a0825822e",
    "snapshot": {
      "displayName": "lele",
      "avatarUrl": "wex-temp-avatar.png",
      "repHeroes": [
        {
          "itemId": "886e3db3-079b-4804-ac6a-c7b187ca9e99",
          "templateId": "Character:Mage_Starter_Fire_Fireball_T03",
          "bIsCommander": true,
          "level": 5,
          "skillLevel": 1,
          "upgrades": [0, 0, 0, 0, 0, 0, 0, 0, 0],
          "accountInfo": {
            "level": 7,
            "perks": [0, 2, 2, 1, 0, 1, 0, 0]
          },
          "foilLevel": 0,
          "gearTemplateId": ""
        }
      ],
      "lastPlayTime": "2017-12-09T20:08:20.865Z",
      "numLevelsCompleted": 6,
      "numTerritoriesClaimed": 0,
      "accountLevel": 7,
      "numRepHeroes": 1,
      "isPvPUnlocked": false
    }
  }
]
```
