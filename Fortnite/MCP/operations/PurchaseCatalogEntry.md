# PurchaseCatalogEntry

**Description**: `Purchase an Offer` \
**Profiles**: `common_core`

## Body

```js
{
    "offerId": "", // from offer
    "purchaseQuantity": 1, // how often you want to purchase the offer
    "currency": "", // from offer
    "currencySubType": "", // from offer
    "expectedTotalPrice": 0, // Calculate it
    "gameContext": "GameContext: Frontend.CatabaScreen" // Leave Like this or use an Empty String
}
```
