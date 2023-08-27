## UE Marketplace - Remove Cart Item

URL: https://www.unrealengine.com/marketplace/api/shoppingCart/delete \
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
    "data": true,
    "status": "OK"
}
```