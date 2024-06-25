## Tag Management Service - Override Own Tags

URL: https://tag-management-public-service-prod.identity.live.on.epicgames.com/api/v1/public/accounts/:accountId/tags \
Method: PUT \
Auth Required: Yes (Account Auth)

```json
{
  "tagsToAdd": [
    "d9e00ab236c343268ebc1fe479b960e6",
    "c8eaf7c8365f478e99a20ff70a83e689",
    "9614aa25267041ad8c7d6e17296fdc65"
  ]
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`tagsToAdd`: Array of maximum 3 Tag Ids

---

_Example Response_

```json
{
  "tags": [
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
