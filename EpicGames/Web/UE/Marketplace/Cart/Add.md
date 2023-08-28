## UE Marketplace - Add Cart Item

URL: https://www.unrealengine.com/marketplace/api/shoppingCart \
Method: POST \
Auth Required: Yes

```json
{
    "offerId": ":offer"
}
```

### Parameters

`offer`: Offer Id

---

_Example Response_

```json
{
    "status": "OK",
    "data": [
        "1e0699cf59d64105957b4aa40f367252"
    ]
}
```