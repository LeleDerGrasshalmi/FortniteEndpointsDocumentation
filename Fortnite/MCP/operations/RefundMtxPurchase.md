# RefundMtxPurchase

**Description**: `Refund a Offer purchased with VBucks` \
**Profiles**: `common_core`

## Body

```js
{
    "purchaseId": "{purchaseId}", // From Purchase History
    "quickReturn": false, // Whether it requires a Refund Token (from profile)
    "gameContext": "Frontend.AthenaLobby" // Leave like this or an Empty String
}
```
