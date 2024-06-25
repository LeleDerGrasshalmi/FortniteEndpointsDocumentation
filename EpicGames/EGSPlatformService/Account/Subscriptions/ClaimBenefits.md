## EGS Platform Service - Claim Subscription Benefits

URL: https://egs-platform-service.store.epicgames.com/api/v1/private/egs/account/subscriptions/claim-benefit \
Method: POST \
Auth Required: Yes (apparently `subscription:public:{accountId}:claim-benefit CREATE`)

```json
{
  "offerId": "a",
  "sandboxId": "b",
  "store": "EGS"
}
```

## Parameters

`offerId`: (required) The offer id from catalog service of the `SUBSCRIPTION` offer <br/>
`sandboxId`: (required) The sandbox namespace of the catalog offer <br/>
`store`: (apparently required) the store of the catalog offer, e.g. `EGS`

---

_Example Response (invalid request)_

```json
{
  "errorMessage": "Failed to get account subscriptionBenefitClaim"
}
```
