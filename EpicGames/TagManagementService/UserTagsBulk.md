## Tag Management Service - User Tags (Bulk)

URL: https://tag-management-public-service-prod.identity.live.on.epicgames.com/api/v1/public/accounts \
Method: GET \
Auth Required: Yes (Account Auth)

## Query Parameters

`accountId`: (required), Account Id of the friend, can be used multiple times

---

_Example Response_

```json
{
  "accounts": [
    {
      "accountId": "94b1569506b04f9f8557af611e8c5e47",
      "tags": [
        {
          "id": "c8eaf7c8365f478e99a20ff70a83e689",
          "name": "BR - Trios",
          "types": ["Game Modes"],
          "primary": false,
          "locale": "en-US",
          "defaultLocaleName": "BR - Trios"
        },
        {
          "id": "9614aa25267041ad8c7d6e17296fdc65",
          "name": "BR - Squads",
          "types": ["Game Modes"],
          "primary": false,
          "locale": "en-US",
          "defaultLocaleName": "BR - Squads"
        },
        {
          "id": "d9e00ab236c343268ebc1fe479b960e6",
          "name": "BR - Duos",
          "types": ["Game Modes"],
          "primary": false,
          "locale": "en-US",
          "defaultLocaleName": "BR - Duos"
        }
      ]
    },
    {
      "accountId": "9d58d46c633f475e8f329d203b7a4198",
      "tags": [
        {
          "id": "2988d22ef475408f8ff4987732192829",
          "name": "Open",
          "types": ["Competitive"],
          "primary": false,
          "locale": "en-US",
          "defaultLocaleName": "Open"
        },
        {
          "id": "9614aa25267041ad8c7d6e17296fdc65",
          "name": "BR - Squads",
          "types": ["Game Modes"],
          "primary": false,
          "locale": "en-US",
          "defaultLocaleName": "BR - Squads"
        },
        {
          "id": "d6dceed8e1dc487dbabef90911d576d5",
          "name": "Cosmetic Cup",
          "types": ["Competitive"],
          "primary": false,
          "locale": "en-US",
          "defaultLocaleName": "Cosmetic Cup"
        }
      ]
    }
  ]
}
```
