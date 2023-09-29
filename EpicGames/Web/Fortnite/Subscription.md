## Fortnite Website - Subscription

URL: https://fortnite.com/api/subscription-offer \
Method: GET \
Auth Required: No

---

_Example Response_

```json
{
  "data": {
    "config": [
      {
        "tier": 1,
        "offerId": "9ec21a8d4f744f8b938fbf79d02d40b9",
        "itemId": "c6cb1a1d11f54fab8e17301f66bc27a4",
        "entitlement": "FN_Crew",
        "slug": "fortnite-subs"
      }
    ],
    "isFounder": false,
    "offers": [
      {
        "0": {
          "id": "9ec21a8d4f744f8b938fbf79d02d40b9",
          "catalogItemId": "c6cb1a1d11f54fab8e17301f66bc27a4",
          "namespace": "fn",
          "title": "Fortnite Crew",
          "recurrence": "SUBSCRIPTION",
          "billingCycle": "MONTHLY",
          "currencyCode": "AUD",
          "priceValue": 1755,
          "discountPriceValue": 1755,
          "discountPercentage": 100,
          "free": false,
          "discounted": false,
          "viewableDate": "2020-12-02T04:45:00.000Z",
          "effectiveDate": "2020-12-02T04:45:00.000Z",
          "seller": {
            "id": "o-aa83a0a9bc45e98c80c1b1c9d92e9e",
            "name": "Epic Games"
          },
          "description": "Join the Fortnite Crew and get these monthly rewards.\n\n- Always own the current season's Battle Pass. Yours to keep. \n- Crew Pack that is exclusive to Fortnite Crew (at least 1,500 V-Bucks in value). \n- Collect 1,000 V-Bucks every month!",
          "longDescription": "Join the Fortnite Crew and get these monthly rewards.\n\n- Always own the current season's Battle Pass. Yours to keep. \n- Crew Pack that is exclusive to Fortnite Crew (at least 1,500 V-Bucks in value). \n- Collect 1,000 V-Bucks every month!\n\nYou may cancel your subscription at any time, without losing access to any of the items received during your subscription. Subscription V-Bucks do not transfer to other platforms.  \n\nRecurring subscription fee charged monthly until cancelled. See full terms on www.fortnite.com/fortnite-crew-terms",
          "featured": false,
          "isCatalogItem": false,
          "categories": [
            {
              "path": "testing"
            }
          ],
          "bundle": false,
          "releaseInfo": [],
          "urlSlug": "fortnite-subs",
          "purchaseLimit": 1,
          "customAttributes": {},
          "tax": 0,
          "tags": [],
          "price": "A$17.55",
          "discount": "A$0.00",
          "discountPrice": "A$17.55"
        },
        "owned": false,
        "ownedCount": 0,
        "canPurchase": false
      }
    ]
  }
}
```
