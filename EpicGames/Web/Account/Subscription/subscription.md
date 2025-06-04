## Account Web - Subscription: Subscription

URL: https://www.epicgames.com/account/v2/subscription/subscription \
Method: GET \
Auth Required: Yes

## Query Parameters

`subscriptionId`: Subscription to find

---

_Example Response_

```json
{
  "elements": [
    {
      "id": "28e3422b50a04d6dacc39423a15a6aee",
      "subscriptionDefId": "eb33b85aec274b5383696f94cef88923",
      "offerId": "9ec21a8d4f744f8b938fbf79d02d40b9",
      "namespace": "fn",
      "inFreePeriod": false,
      "isNonRenewing": false,
      "subscriptionStatus": "EXPIRED",
      "isAutoRenewEnabled": false,
      "endDate": "2023-04-30T20:28:20.522+0000",
      "billingCycle": "MONTHLY",
      "transactionFailed": false,
      "title": "Fortnite Crew",
      "author": "Epic Games",
      "thumbnail": "https://cdn1.epicgames.com/fn/offer/MasterArt_512x512_Logo-512x512-e6eaaf5fe24d353db3d331690196a1f8.jpg",
      "offerPrice": 1199,
      "priceString": "€11.99",
      "endDateMillis": 1682886500522,
      "createdAtMillis": 1680294500522,
      "nextBillingDateMillis": 1682886500522
    }
  ]
}
```
