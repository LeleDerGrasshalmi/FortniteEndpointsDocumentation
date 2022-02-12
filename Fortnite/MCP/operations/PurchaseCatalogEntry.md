# PurchaseCatalogEntry

**Description**: `Purchase a Catalog Entry, specified via OfferId` \
**Profiles**: `common_core`

## Body
```js
{
    "offerId": "", //the offerId (=> which CatalogEntry you want to purchase)
    "purchaseQuantity": 1, //the quantity (how often you want to purchase it, should be normally 1)
    "currency": "MtxCurrency", //the currency
    "currencySubType": "", //the currency subtype, leave empty is not existing
    "expectedTotalPrice": 0, //calculate urself
    "gameContext": "GameContext: Frontend.CatabaScreen" //leave it empty, or like this
}
```
