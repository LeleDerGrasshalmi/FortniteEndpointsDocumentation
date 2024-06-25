## Tag Management Service - Own Tags

URL: https://tag-management-public-service-prod.identity.live.on.epicgames.com/api/v1/public/accounts/:accountId/tags \
Method: GET \
Auth Required: Yes (Account Auth)

## Path Parameters

`accountId`: Your Account Id

---

_Example Response_

```json
{
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
}
```
