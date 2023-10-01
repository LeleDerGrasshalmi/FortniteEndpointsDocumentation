## UE Marketplace - Tracking Info

URL: https://www.unrealengine.com/marketplace/api/purchase/track \
Method: POST \
Auth Required: Yes

```json
{
  "offerId": [":offer"],
  "purchaseFlow": 1
}
```

## Parameters

`offerId`: The Ids of the Offers <br/>
`purchaseFlow`: Random Tracking ID

---

_Example Response_

```json
{
  "status": "OK",
  "data": true
}
```
