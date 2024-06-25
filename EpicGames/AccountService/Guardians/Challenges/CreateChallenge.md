## Account Service - Guardians: Create Guardian Challenge

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/guardians/challenges \
Method: POST \
Auth Required: Yes (`account:public:guardians CREATE`)

```json
{
  "guardianEmail": "lele@example.com"
}
```

## Parameters

`guardianEmail`: Email of the guardian

---

_Example Response: (No Birth Date)_

```json
{
  "errorCode": "errors.com.epicgames.account.date_of_birth_not_set",
  "errorMessage": "Sorry, the date of birth for account 94b1569506b04f9f8557af611e8c5e47 is not set.",
  "messageVars": ["94b1569506b04f9f8557af611e8c5e47"],
  "numericErrorCode": 18222,
  "originatingService": "com.epicgames.account.public",
  "intent": "prod"
}
```
