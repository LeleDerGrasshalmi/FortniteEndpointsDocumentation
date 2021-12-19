# GiftCatalogEntry

**Description**: `Gifts a Catalog Entry to specified users` \
**Profiles**: `common_core`

## Body
```js
{
    "offerId": "{offerId}", //the offerId (=> which CatalogEntry you want to gift)
    "currency": "MtxCurrency", //leave it like this
    "currencySubType": "", //leave empty
    "expectedTotalPrice": 0, //calculate urself
    "gameContext": "Frontend.CatabaScreen", //leave it like this
    "receiverAccountIds": [], //array of accountIds of the people that should recieve the gift
    "giftWrapTemplateId": "", //leave it empty, or choose between these: GiftBox:GB_GiftWrap1 (1-4)
    "personalMessage": "" //not used ingame anymore, but works
}
```
