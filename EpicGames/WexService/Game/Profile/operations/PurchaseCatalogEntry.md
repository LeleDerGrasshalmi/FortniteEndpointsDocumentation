# PurchaseCatalogEntry

**Description**: `Purchases an offer from the catalog` \
**Profiles**: `profile0`

## Body

```js
{
    "offerId": "", // GUID of the offer to purchase
    "purchaseQuantity": 0, // Amount of the offer to purchase
    "currency": "", // Currency to use for the purchase
    "currencySubType": "", // Subtype of the currency to use for the purchase
    "expectedTotalPrice": 0, // Expected price of the purchase
    "gameContext": "" // Context of the purchase
}
```
