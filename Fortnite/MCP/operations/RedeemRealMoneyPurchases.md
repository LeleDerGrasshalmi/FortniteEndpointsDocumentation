# RedeemRealMoneyPurchases

**Description**: `Claims Real Money Purchase Items` \
**Profiles**: `common_core`

## Body

```js
{
    "appStore": "EpicPurchasingService", // e.g. EpicPurchasingService
    "authTokens": [], // Auth Token (Included in the Auth Response or requested using the platformtoken api) - Required for all app Stores expect EpicPurchasingService & SamsungGalaxyAppStore
    "receiptIds": [], // Receipt Ids, if you just want to refresh those
    "refreshType": "ForceCurrent", // Enum: Default, UpdateOfflineAuth, ForceAll, ForceCurrent
    "verifierModeOverride": "DefaultToConfig", // Unknown and DefaultToConfig was used in the request I captured (fn v24.20), but Enum values: OccurrencePrimary, ReceiptOnly, ReceiptPrimary, DefaultToIapVersion, OccurrenceOnly, DefaultToConfig, OccurrenceOnlyRemoveReceipts
    "purchaseCorrelationId": "" // Can be ignored
}
```
