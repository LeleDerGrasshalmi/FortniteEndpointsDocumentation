# PurchaseCatalogEntry

**Description**: `Purchase an Offer` \
**Profiles**: `common_core`

## Body

```js
{
    "offerId": "", // From offer
    "purchaseQuantity": 1, // How often you want to purchase the offer
    "currency": "", // From offer
    "currencySubType": "", // From offer
    "expectedTotalPrice": 0, // Calculate it
    "gameContext": "GameContext: Frontend.CatabaScreen", // Leave like this or use an empty string
    "client_request_id": "", // Optional - Unique request identifier
    "additionalData": { // Optional - Extra context for the purchase
        "islandId": "", // Optional - e.g. "campaign"
        "islandTitle": "", // Optional - e.g. "None"
        "productTag": "", // Optional - e.g. "Product.STW"
        "storeContext": "", // Optional - e.g. "FrontEnd"
        "sourceContext": "", // Optional
        "checkoutProperties": {}, // Optional - Additional checkout metadata
        "itemShopFilterContext": { // Optional - Active/inactive filter state
            "activeFilters": [],
            "inactiveFilters": []
        },
        "storeFront": "", // Optional - e.g. "CardPackStoreGameplay"
        "storeId": "", // Optional
        "groupId": "" // Optional
    }
}
```
