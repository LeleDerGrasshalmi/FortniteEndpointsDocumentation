## UE Marketplace - SSO Info

URL: https://www.unrealengine.com/marketplace/api/sso \
Method: GET \
Auth Required: Yes

---

_Example Response_

```json
{
  "status": "OK",
  "data": {
    "id": "id here",
    "displayName": "test",
    "name": "test",
    "email": "test@gmail.com",
    "failedLoginAttempts": 0,
    "lastLogin": "2023-08-26T09:31:15.090Z",
    "numberOfDisplayNameChanges": 3,
    "ageGroup": "UNKNOWN",
    "headless": false,
    "country": "AU",
    "lastName": "mm",
    "preferredLanguage": "en",
    "lastDisplayNameChange": "2022-12-16T20:27:19.812Z",
    "canUpdateDisplayName": true,
    "tfaEnabled": false,
    "emailVerified": true,
    "minorVerified": false,
    "minorExpected": false,
    "minorStatus": "NOT_MINOR",
    "cabinedMode": false,
    "hasHashedEmail": false,
    "isLoggedIn": true
  }
}
```