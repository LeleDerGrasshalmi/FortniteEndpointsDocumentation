# VerifyRealMoneyPurchase

**Description**: `Verifies a specified Receipt/Real Money Purchase` \
**Profiles**: `common_core`

## Body

```js
{
    "appStore": "", // from receipt, e.g. EpicPurchasingService
    "appStoreId": "", // from receipt
    "receiptId": "", // from receipt
    "receiptInfo": "", // from receipt
    "purchaseCorrelationId": "" // not needed & not known where it comes from (maybe from purchase request headers?)
}
```

[**Get All Receipts**](../../Catalog/Receipts.md)
