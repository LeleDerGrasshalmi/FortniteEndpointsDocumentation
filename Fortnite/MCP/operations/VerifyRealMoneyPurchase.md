# VerifyRealMoneyPurchase

**Description**: `Verifies a specified Receipt/Real Money Purchase` \
**Profiles**: `common_core`

## Body

```js
{
    "appStore": "", // From Receipt, e.g. EpicPurchasingService
    "appStoreId": "", // From Receipt
    "receiptId": "", // From Receipt
    "receiptInfo": "", // From Receipt
    "purchaseCorrelationId": "" // Not needed & not known where it comes from (maybe from purchase request headers?)
}
```

--> [**Get All Receipts**](../../Catalog/Receipts.md)
