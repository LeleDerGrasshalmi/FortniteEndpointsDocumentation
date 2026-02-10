## Account Web - Order: Refundability

URL: https://www.epicgames.com/account/v2/order/refundability \
Method: GET \
Auth Required: Yes

## Query Parameters

`orderId`: The Id of the Order

---

_Example Response_

```json
{
  "data": {
    "refundable": false,
    "lineOffers": {
      "0ee146487aa14105bfab7bf76029ef6a": {
        "refundable": false,
        "refunded": false
      }
    }
  },
  "orderId": "F9504250112456806"
}
```
