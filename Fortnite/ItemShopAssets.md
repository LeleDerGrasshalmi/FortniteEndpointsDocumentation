## Fortnite - ItemShop Assets [deprecated]

URL: https://www.epicgames.com/graphql \
Method: POST \
Auth Required: No

## Body

```json
{
  "query": "query FortniteQuery { Fortnite { getCurrentStoreOffers { storefronts { catalogEntries { assetName } } success } } }"
}
```

## Requesting the Image

`GET` `https://cdn2.unrealengine.com/Kairos/itemShopAssets/:assetName`
e.g. `https://cdn2.unrealengine.com/Kairos/itemShopAssets/glider_id_7e2feac303d7bd4f8a33ff77db22fdc9ea19342cbd95f830d002080e6b1deef2.jpg`
![Chinese 2k Vucks Glider](https://cdn2.unrealengine.com/Kairos/itemShopAssets/glider_id_7e2feac303d7bd4f8a33ff77db22fdc9ea19342cbd95f830d002080e6b1deef2.jpg)
