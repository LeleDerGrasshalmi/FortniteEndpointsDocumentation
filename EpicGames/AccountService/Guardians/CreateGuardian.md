## Account Service - Guardians: Create Guardian

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/guardians \
Method: POST \
Auth Required: Yes (`account:public:guardians CREATE`)

> This API has been deprecated/removed

```json
{
  "guardianEmail": "lele@example.com",
  "country": "DE",
  "dateOfBirth": "2000-12-06"
}
```

## Parameters

`guardianEmail`: Email of the guardian <br/>
`country`: ISO 3166 - Alpha 2 Code of the guardian <br/>
`dateOfBirth`: Date of birth of the account

---

_Example Response: (Success)_

```json
{
  "id": "b9cf8da3fac74e92bd15ce5d6dee1101",
  "guardianEmail": "lele@example.com",
  "dateOfBirth": "2000-12-06",
  "country": "DE",
  "childAccountId": "94b1569506b04f9f8557af611e8c5e47",
  "guardianAccountId": "acfe2f3787fd46eab3ce3614efcdb70e",
  "clientId": "3446cd72694c4a4485d81b77adbb2141",
  "createdAt": "2022-12-11T09:55:47.341Z",
  "deadline": "2023-01-10T09:55:47.341Z",
  "completed": false,
  "guardianLastEmailed": "2022-12-11T09:55:47.350Z",
  "emailChallenged": false,
  "createdExternally": true
}
```
