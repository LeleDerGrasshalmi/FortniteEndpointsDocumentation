# VerifyRealMoneyPurchase

**Description**: `Verifies a receipt for a purchase and refreshes the profile` \
**Profiles**: `profile0`

## Body

```js
{
    "appStore": "", // App Store the purchase was made on (DebugStore, EpicPurchasingService, IOSAppStore, WeGameStore, GooglePlayAppStore, KindleStore, PlayStationStore, XboxLiveStore, NintendoEShop, SamsungGalaxyAppsStore)
    "appStoreId": "", // App Store ID of the item purchased (e.g. bb_viptier2_release)
    "receiptId": "", // Receipt ID of the purchase
    "receiptInfo": "", // Receipt data (String of JSON containing receiptData and signature)
    "purchaseCorrelationId": "" // Correlation ID of request that made the purchase
}
```
