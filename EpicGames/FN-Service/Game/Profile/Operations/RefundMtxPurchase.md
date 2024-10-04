# RefundMtxPurchase

**Description**: `Refund an offer purchased with V-Bucks` \
**Profiles**: `common_core`

## Body

```js
{
    "purchaseId": "", // The purchaseId from Purchase History (Profile Stat)
    "quickReturn": false, // Whether to use the Cancel Purchase feature
    "gameContext": "Frontend.AthenaLobby" // Leave like this or an empty string
}
```
