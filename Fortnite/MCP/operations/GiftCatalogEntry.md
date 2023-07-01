# GiftCatalogEntry

**Description**: `Gift a Catalog Offer to friends` \
**Profiles**: `common_core`

## Body

```js
{
    "offerId": "", // From offer
    "currency": "", // From offer
    "currencySubType": "", // From offer
    "expectedTotalPrice": 0, // Calculate yourself or let epic calc it (using their endpoint)
    "gameContext": "Frontend.CatabaScreen", // Leave or Empty String
    "receiverAccountIds": [], // Friends Account Ids
    "giftWrapTemplateId": "", // Empty String
    "personalMessage": "" // Not used anymore (also doesnt show ingame anymore since v23.00)
}
```
