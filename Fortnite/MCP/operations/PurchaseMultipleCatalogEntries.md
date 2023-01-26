# PurchaseMultipleCatalogEntries

**Description**: `Purchase Catalog Entries (Bulk)` \
**Profiles**: `common_core`

## Body

```js
{
    "purchaseInfoList": [{
        "offerId": "", // From offer
        "purchaseQuantity": 1, // How often you want to purchase the offer
        "currency": "", // From offer
        "currencySubType": "", // From offer
        "expectedTotalPrice": 0, // Calculate it
        "gameContext": "GameContext: Frontend.CatabaScreen" // Leave Like this or use an Empty String
    }]
}
```
