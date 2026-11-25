## EGS Platform Service - Account: Wallet

URL: https://egs-platform-service.store.epicgames.com/api/v1/private/egs/account/wallet <br/>
Method: GET <br/>
Auth Required: Yes (apparently `reward:public:{accountId}:reward-accounts	READ`)

## Query Parameters

`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`store`: (required) valid Catalog Service Stores, e.g. `EGS`

---

*Example Response (missing perm)*

```json
{
  "errorMessage": "Unauthorized"
}
```

*Example Response (success)*

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
