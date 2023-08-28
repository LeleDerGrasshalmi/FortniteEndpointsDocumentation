## UE Marketplace - Tracking Info

URL: https://www.unrealengine.com/marketplace/api/purchase/track \
Method: POST \
Auth Required: Yes

```json
{
    "offerId": [
        ":offer"
    ],
    "purchaseFlow": 1
}
```

## Parameters

`offer`: the Id of the Offer <br/>
`purchaseFlow`: random tracking id

---

_Example Response_

```json
{
    "status": "OK",
    "data": true
}
```