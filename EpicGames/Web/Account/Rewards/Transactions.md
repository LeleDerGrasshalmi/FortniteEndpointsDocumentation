## Account Web - Rewards: Transactions

URL: https://www.epicgames.com/account/v2/reward-account/transactions \
Method: GET \
Auth Required: Yes

## Query Parameters

`nextPageToken`: From the previous Request <br/>
`count`: How many Elements should be returned <br/>
`locale`: Content Language

---

_Example Response (shortened)_

```json
{
  "transactions": [
    {
      "priceString": "€0.60",
      "offers": [
        {
          "description": "Fortnite Crew"
        }
      ],
      "marketplaceName": "Fortnite",
      "createdAtMillis": 1693762253000,
      "transactionType": "EARN",
      "direction": "+",
      "id": "101f3607aa124cec8ddb51dc92be4baf"
    }
  ],
  "nextPageToken": "next-2023-06-03T17:30:54Z",
  "count": 10
}
```
