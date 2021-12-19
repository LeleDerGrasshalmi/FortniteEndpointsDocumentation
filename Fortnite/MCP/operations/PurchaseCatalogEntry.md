# PurchaseCatalogEntry

**Description**: `Purchase a Catalog Entry, specified via OfferId` \
**Profiles**: `common_core`

## Body
```js
{
    "offerId": "v2:/d4839382b66817e72d6461866545153b251cf6707667caea6acfe068692c83c5", //the offerId (=> which CatalogEntry you want to purchase)
    "purchaseQuantity": 1, //the quantity (how often you want to purchase it, should be normally 1)
    "currency": "MtxCurrency", //leave it like this
    "currencySubType": "", //leave empty
    "expectedTotalPrice": 0, //calculate urself
    "gameContext": "GameContext: Frontend.CatabaScreen" //leave it empty, or like this
}
```
