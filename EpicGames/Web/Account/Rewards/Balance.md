## Account Web - Rewards: Balance

URL: https://www.epicgames.com/account/v2/reward-account \
Method: GET \
Auth Required: Yes

## Query Parameters

`currency`: Currency Format, defaults to `USD` <br/>
`locale`: Number Representation, defaults to `en-US`

---

_Example Response (shortened)_

```json
{
  "totalAvailableBalancePriceString": "€6.00",
  "totalPendingBalancePriceString": "€0.00",
  "soonestExpiringBalancePriceString": "€0.60",
  "expirationDate": 1752710400000
}
```
