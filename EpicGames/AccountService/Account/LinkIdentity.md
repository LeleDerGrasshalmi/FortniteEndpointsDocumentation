## Account Service - Set Link Identity Type

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId/linkIdentity \
Method: POST \
Auth Required: Yes (`account:public:account:linkedIdentity CREATE`)

```json
{
  "type": "unknown",
  "value": "something"
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`type`: Unknown Value <br/>
`value`: Unknown Value

---

_Example Response (Invalid Type)_

```json
{
  "errorCode": "errors.com.epicgames.bad_request",
  "errorMessage": "type TYPE is not supported to link",
  "messageVars": ["TYPE"],
  "numericErrorCode": 1001,
  "originatingService": "com.epicgames.account.public",
  "intent": "prod"
}
```
