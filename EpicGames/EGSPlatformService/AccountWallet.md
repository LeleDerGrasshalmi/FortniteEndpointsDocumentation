## EGS Platform Service - Account Wallet

URL: https://egs-platform-service.store.epicgames.com/api/v1/private/egs/account/wallet \
Method: GET \
Auth Required: Yes (apparently `reward:public:{accountId}:reward-accounts	READ`)

## Query Parameters

`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`store`: (required) valid Catalog Stores, e.g. `EGS`, `NONE` <br/>

---

Example Response

```json
{
  "coupons": {
    "count": 0
  },
  "epicRewards": {
    "__typename": "EpicRewardsSupported",
    "balance": "€0.00"
  },
  "wallet": {
    "__typename": "EpicWalletSupported",
    "balance": "€0.00"
  }
}
```
