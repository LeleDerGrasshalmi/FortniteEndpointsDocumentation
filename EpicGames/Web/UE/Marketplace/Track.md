## UE Marketplace - Tracking Info

URL: https://www.unrealengine.com/marketplace/api/purchase/track <br/>
Method: POST <br/>
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

*Example Response*

```json
{
  "status": "OK",
  "data": true
}
```
