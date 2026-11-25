## Account Service - Guardians: Send Guardian Challenge Notification

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/guardians/challenges/:challengeId/notifications <br/>
Method: POST <br/>
Auth Required: Yes (`account:public:guardians CREATE`)

## Path Parameters

`challengeId`: The Challenge Id gotten from creating the challenge or from fetching the latest challenge

---

*Example Response: (Challenge not found)*

```json
{
  "errorCode": "errors.com.epicgames.account.guardian_challenge_not_found",
  "errorMessage": "Sorry, we couldn't find guardian challenge with id: b9cf8da3fac74e92bd15ce5d6dee1101",
  "messageVars": ["b9cf8da3fac74e92bd15ce5d6dee1101"],
  "numericErrorCode": 18142,
  "originatingService": "com.epicgames.account.public",
  "intent": "prod"
}
```
