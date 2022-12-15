# GiftCatalogEntry

**Description**: `Gift a Catalog Offer to friends` \
**Profiles**: `common_core`

## Body

```js
{
    "offerId": "", //th from offer
    "currency": "", // from offer
    "currencySubType": "", // from offer
    "expectedTotalPrice": 0, // Calculate yourself or let epic calc it (using their endpoint)
    "gameContext": "Frontend.CatabaScreen", // Leave or Empty String
    "receiverAccountIds": [], // Friends Account Ids
    "giftWrapTemplateId": "", // Empty String or GiftBox:GB_GiftWrap1 (1-4)
    "personalMessage": "" // Not used anymore (also doesnt show ingame anymore since v23.00)
}
```
