## UE Web - List

URL: https://www.unrealengine.com/marketplace/api/shoppingCart \
Method: GET \
Auth Required: No

## Query Parameters

`calculatePrice`: show price and detail (boolean)

---

_Example Response_

```json
{
  "status": "OK",
  "data": {
    "offerIds": ["1e0699cf59d64105957b4aa40f367252"],
    "totalPrice": "$25.74",
    "totalPriceDisplay": {
      "amount": "25.74",
      "symbol": "$",
      "placement": "f",
      "digits": 2
    }
  }
}
```