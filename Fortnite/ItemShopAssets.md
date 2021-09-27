## Fortnite - ItemShop Assets

URL: https://www.epicgames.com/graphql \
Method: POST \
Auth Required: No

## Body
```json
{
    "query": "query FortniteQuery {Fortnite {getCurrentStoreOffers {storefronts {catalogEntries { assetName}}success}}}"
}
```
