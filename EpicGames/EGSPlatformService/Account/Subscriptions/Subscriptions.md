## EGS Platform Service - Subscriptions

URL: https://egs-platform-service.store.epicgames.com/api/v1/private/egs/account/subscriptions \
Method: GET \
Auth Required: Yes (apparently `subscription:public:{accountId}:subscription READ`)

## Query Parameters

`count`: (required) element count to return <br/>
`start`: (required) start index <br/>
`sandboxId`: (optional) only include subscriptions from the specified sandbox <br/>
`sortDirection`: (optional) sort the results, by `ASC` or `DESC`

---

_Example Response (missing perm)_

```json
{
  "errorMessage": "Failed to get account accountSubscription"
}
```

_Example Response (success)_

```json
{
  "paging": {
    "count": 1,
    "start": 0,
    "total": 1
  },
  "subscriptions": [
    {
      "billing": {
        "billingCycle": "MONTHLY",
        "countryCode": "DE",
        "endDate": "2024-06-03T17:30:44.370+0000",
        "inDunning": false,
        "inFreePeriod": false,
        "isAutoRenewEnabled": true,
        "isNonRenewing": false,
        "nextBillingDate": "2024-06-03T17:30:44.370+0000"
      },
      "id": "b2f8bc8c2c4e4aa3a002e2dff17d5baa",
      "subscription": {
        "levelItemId": "c6cb1a1d11f54fab8e17301f66bc27a4",
        "offerId": "9ec21a8d4f744f8b938fbf79d02d40b9",
        "sandboxId": "fn"
      },
      "subscriptionStatus": "ACTIVE"
    }
  ]
}
```
