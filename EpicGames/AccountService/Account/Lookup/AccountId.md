## Account Service - Lookup by Account Id

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId \
Method: GET \
Auth Required: Yes (`account:public:account READ`)

## Path Parameters

`accountId`: The Target Account Id to lookup

---

_Example Response (Own Account)_

```json
{
  "id": "94b1569506b04f9f8557af611e8c5e47",
  "displayName": "lele stw moment",
  "name": "ABC",
  "email": "lele@example.com",
  "failedLoginAttempts": 0,
  "lastLogin": "2023-05-02T16:51:59.221Z",
  "numberOfDisplayNameChanges": 1,
  "ageGroup": "UNKNOWN",
  "headless": false,
  "country": "DE",
  "lastName": "ABC",
  "phoneNumber": "12345667890",
  "company": "Lele Exploits",
  "preferredLanguage": "de",
  "lastDisplayNameChange": "2022-09-10T08:07:47.361Z",
  "canUpdateDisplayName": true,
  "tfaEnabled": true,
  "emailVerified": true,
  "minorVerified": false,
  "minorExpected": false,
  "minorStatus": "NOT_MINOR",
  "guardianChallengeTimestamp": "2023-03-18T20:26:07.806Z",
  "siweNotificationEnabled": true,
  "cabinedMode": false,
  "hasHashedEmail": false,
  "lastReviewedSecuritySettings": "2024-12-11T11:46:48.381Z"
}
```

_Example Response (Not Own Account)_

```json
{
  "id": "94b1569506b04f9f8557af611e8c5e47",
  "displayName": "lele stw moment",
  "externalAuths": {}
}
```
