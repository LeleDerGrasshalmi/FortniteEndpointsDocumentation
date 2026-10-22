# GiftCatalogEntry

**Description**: `Gift a Catalog Offer to friends` \
**Profiles**: `common_core`

## Body

```js
{
    "offerId": "", // From catalog offer
    "currency": "", // From catalog offer
    "currencySubType": "", // From catalog offer
    "expectedTotalPrice": 0, // Leave or get discounted price(s) from catalog offer
    "gameContext": "Frontend.CatabaScreen", // Leave or Empty String (where the purchase was made)
    "receiverAccountIds": [], // Friends Account Ids
    "giftWrapTemplateId": "", // Empty String, GiftBox:gb_default (purple), or GiftBox:gb_giftwrap1 (1: red, 2: yellow, 3: blue)
    "personalMessage": "" // Not used anymore (also doesnt show ingame anymore since v23.00)
}
```
