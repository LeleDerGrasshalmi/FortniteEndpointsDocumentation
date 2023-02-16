# RedeemRealMoneyPurchases

**Description**: `Claims Real Money Purchase Items` \
**Profiles**: `common_core`

## Body

```js
{
    "appStore": "EpicPurchasingService", // e.g. EpicPurchasingService
    "authTokens": [], // Auth Token (Included in the Auth Response) - Required for all app Stores expect EpicPurchasingService & SamsungGalaxyAppStore
    "receiptIds": [], // Receipt Ids, if you just want to refresh those
    "refreshType": "ForceCurrent", // Enum: ForceCurrent, ForceAll, Default, UpdateOfflineAuth
    "purchaseCorrelationId": "" // Can be ignored
}
```
