## Fulfillment Service - Redeem Code (Account)

URL: https://fulfillment-public-service-prod.ol.epicgames.com/fulfillment/api/public/accounts/:accountId/codes/:code \
Method: POST \
Auth Required: Yes (`fulfillment:public:code CREATE`)

## Path Parameters

`accountId`: Your account id <br/>
`code`: The redemption code, without dashes

---

_Example Response_

```json
{
  "offerId": "5ae93cd2ca5244b6827bb1220ccbdd8d",
  "accountId": "5f38c3127c8f44f9b59ae33b095d60b0",
  "identityId": "5f38c3127c8f44f9b59ae33b095d60b0",
  "details": [
    {
      "entitlementId": "54d6793c97b2404c89699392ac9c9d2e",
      "entitlementName": "FN_Potassium_Emote",
      "itemId": "279dc3910ae849a7b223da0fac321868",
      "namespace": "fn",
      "country": "DE"
    }
  ]
}
```

_Example Response (Multi redeem not allowed)_

```json
{
  "errorCode": "errors.com.epicgames.coderedemption.multiple_redemptions_not_allowed",
  "errorMessage": "Multiple redemptions are not allowed for the same user; code:BANANNANANANA, userId: c735bafd3c4c4a6190c4bfb1dedfbef0",
  "messageVars": ["BANANNANANANA", "c735bafd3c4c4a6190c4bfb1dedfbef0"],
  "numericErrorCode": 19025,
  "originatingService": "com.epicgames.fulfillment.public",
  "intent": "prod"
}
```
