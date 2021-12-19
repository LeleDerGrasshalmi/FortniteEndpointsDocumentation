# RefundMtxPurchase

**Description**: `Refunds a purchase` \
**Profiles**: `common_core`

## Body
```js
{
    "purchaseId": "{purchaseId}", //specifies the purchase to refund
    "quickReturn": false, //whether its returned soon after purchase, or in the refund menue
    "gameContext": "Frontend.AthenaLobby" //leave it like this
}
```
