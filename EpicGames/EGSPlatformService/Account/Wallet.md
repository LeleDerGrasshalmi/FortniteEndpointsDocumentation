## EGS Platform Service - Account: Wallet

URL: https://egs-platform-service.store.epicgames.com/api/v1/private/egs/account/wallet \
Method: GET \
Auth Required: Yes (apparently `reward:public:{accountId}:reward-accounts	READ`)

## Query Parameters

`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`store`: (required) valid Catalog Service Stores, e.g. `EGS`

---

_Example Response (missing perm)_

```json
{
  "errorMessage": "Unauthorized"
}
```

_Example Response (success)_

```json
{
  "__typename": "Wallet",
  "coupons": {
    "count": 0
  },
  "epicRewards": {
    "__typename": "EpicRewardsSupported",
    "balance": "€9.63",
    "rawBalance": 963
  },
  "wallet": {
    "__typename": "EpicWalletSupported",
    "balance": "€0.00"
  }
}
```
