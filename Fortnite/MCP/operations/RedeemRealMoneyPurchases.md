# RedeemRealMoneyPurchases

**Description**: `Verifies Purchases from an specified App Store` \
**Profiles**: `common_core`

## Body

```js
{
    "appStore": "EpicPurchasingService", // e.g. EpicPurchasingService
    "authTokens": [], // Auth Token (issued by the external platform ig) - Used for all app Stores expect EpicPurchasingService & SamsungGalaxyAppStore
    "receiptIds": [], // Receipt Ids, if you just want to refresh those
    "refreshType": "ForceCurrent", // Enum: ForceCurrent, ForceAll, Default, UpdateOfflineAuth
    "purchaseCorrelationId": "" // can be ignored
}
```
