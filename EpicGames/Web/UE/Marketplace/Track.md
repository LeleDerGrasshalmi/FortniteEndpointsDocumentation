## UE Marketplace - Tracking Info

URL: https://www.unrealengine.com/marketplace/api/purchase/track \
Method: POST \
Auth Required: Yes

## Parameters

`offer`: the Id of the Offer
`purchaseFlow` random tracking id

```json
{
    "offerId": [
        ":offer"
    ],
    "purchaseFlow": 1
}
```

---

_Example Response_

```json
{
    "status": "OK",
    "data": true
}
```