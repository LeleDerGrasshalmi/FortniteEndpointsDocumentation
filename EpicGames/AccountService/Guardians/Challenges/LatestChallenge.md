## Account Service - Guardians: Get Latest Guardian Challenge

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/guardians/challenges <br/>
Method: GET <br/>
Auth Required: Yes (`account:public:guardians READ`)

Note: Has been removed as of September 15th 2026

---

*Example Response: (Success)*

```json
{
  "id": "983cf4a136994a12b75a2e5618392b12",
  "guardianEmail": "lele@example.com",
  "createdAt": "2023-01-30T13:45:34.853Z",
  "lastNotification": {
    "sentAt": "2023-01-30T13:46:09.804Z",
    "canResendAt": "2023-01-31T13:46:09.804Z"
  },
  "completed": false
}
```

*Example Response: (Not minor)*

```json
{
  "errorCode": "errors.com.epicgames.account.account_is_not_minor",
  "errorMessage": "Account 94b1569506b04f9f8557af611e8c5e47 is not minor.",
  "messageVars": ["94b1569506b04f9f8557af611e8c5e47"],
  "numericErrorCode": 18214,
  "originatingService": "com.epicgames.account.public",
  "intent": "prod"
}
```
