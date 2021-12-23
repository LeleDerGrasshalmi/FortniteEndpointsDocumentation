# PurchaseMultipleCatalogEntries

**Description**: `Purchase Catalog Entries (Bulk)` \
**Profiles**: `common_core`

## Body
```js
{
    "PurchaseInfoList": [{
        "offerId": "", //the offerId (=> which CatalogEntry you want to purchase)
        "purchaseQuantity": 1, //the quantity (how often you want to purchase it, should be normally 1)
        "currency": "MtxCurrency", //the currencry
        "currencySubType": "", //the currencry subtype, leave empty is not existing
        "expectedTotalPrice": 0, //calculate urself
        "gameContext": "GameContext: Frontend.CatabaScreen" //leave it empty, or like this
    }]
}
```
