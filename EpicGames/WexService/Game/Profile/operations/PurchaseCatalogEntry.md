# PurchaseCatalogEntry

**Description**: `Purchases an offer from the catalog` \
**Profiles**: `profile0`

## Body

```js
{
    "offerId": "", // GUID of the offer to purchase
    "purchaseQuantity": 0, // Amount of the offer to purchase
    "currency": "", // Currency to use for the purchase (RealMoney, MtxCurrency, GameItem, Other)
    "currencySubType": "", // Subtype of the currency to use for the purchase (Template ID usually)
    "expectedTotalPrice": 0, // Expected price of the purchase
    "gameContext": "" // Context of the purchase
}
```
