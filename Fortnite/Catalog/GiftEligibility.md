## Fortnite - Check Gifting Friend Status

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/storefront/v2/gift/check_eligibility/recipient/:friendId/offer/:offerId \
Method: GET \
Auth Required: Yes (User Auth for FN)

# Path Parameters

`friendId`: Your Friends Account Id <br/>
`offerId`: The Url Encoded Offer Id

---

_Example Response (Not Owned)_

```json
{
  "price": {
    "currencyType": "MtxCurrency",
    "currencySubType": "",
    "regularPrice": 200,
    "dynamicRegularPrice": 200,
    "finalPrice": 200,
    "saleExpiration": "9999-12-31T23:59:59.999Z",
    "basePrice": 200
  },
  "items": [
    {
      "templateId": "AthenaDance:eid_vectorsparkv3",
      "quantity": 1
    }
  ]
}
```
