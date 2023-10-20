## Account Service - Create Account

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account \
Method: POST \
Auth Required: Yes (`account:public:account CREATE`)

```json
{
  "name": "_",
  "lastName": "_",
  "preferredLanguage": "de",
  "displayName": "lele test",
  "phoneNumber": "0123456789",
  "company": "Lele Exploits",
  "email": "lele@exmaple.com",
  "password": "hey123!",
  "dateOfBirth": "2000-12-24"
}
```

## Query Parameters

`authenticate`: Optional, boolean, Should the response include an oauth session? (Default: False) <br/>
`tokenType`: Optional, string, The type for the oauth token (ex. `eg1`) <br/>
`sendEmail` Optional, boolean, Should the email associated receive a verify email? (Default: False)

## Parameters

`name`: Optional, Your Firstname <br/>
`lastName`: Optional, Your Lastname <br/>
`preferredLanguage`: Optional, Your new Preferred Language <br/>
`displayName`: Optional, Your Display Name <br/>
`phoneNumber`: Optional, Your Phone-Number <br/>
`company`: Optional, Your Company <br/>
`email`: Optional, Your Email <br/>
`username`: Optional, Your Username (could be used instead of an email back then) <br/>
`password`: Optional, Your Password (required if email/username is specified) <br/>
`dateOfBirth`: required, Your BirthDate

---

_Example Response (Full Params)_

```json
{
  "accountInfo": {
    "id": "77f023b60d9c4a0784aea535f458ec42",
    "displayName": "lele test",
    "name": "_",
    "email": "lele@exmaple.com",
    "failedLoginAttempts": 0,
    "numberOfDisplayNameChanges": 0,
    "ageGroup": "UNKNOWN",
    "headless": false,
    "country": "DE",
    "lastName": "_",
    "phoneNumber": "0123456789",
    "company": "Lele Exploits",
    "preferredLanguage": "de",
    "canUpdateDisplayName": true,
    "tfaEnabled": false,
    "emailVerified": false,
    "minorVerified": false,
    "minorExpected": false,
    "minorStatus": "NOT_MINOR",
    "cabinedMode": false,
    "hasHashedEmail": false
  }
}
```

_Example Response (Credentials Set)_

```json
{
  "accountInfo": {
    "id": "5bd3a61d0e6846d6b0cd1bd3a00932ff",
    "displayName": "lele test",
    "email": "lele@example.com",
    "failedLoginAttempts": 0,
    "numberOfDisplayNameChanges": 0,
    "ageGroup": "UNKNOWN",
    "headless": false,
    "country": "DE",
    "preferredLanguage": "en",
    "canUpdateDisplayName": true,
    "tfaEnabled": false,
    "emailVerified": false,
    "minorVerified": false,
    "minorExpected": false,
    "minorStatus": "UNKNOWN",
    "cabinedMode": false,
    "hasHashedEmail": false
  },
  "oauthSession": {
    "access_token": "ed883b805ae245f4943a2d4832ef50fe",
    "expires_in": 7200,
    "expires_at": "2023-02-01T23:52:51.234Z",
    "token_type": "bearer",
    "refresh_token": "55e74c5692ab4c08a0714791814f72ac",
    "refresh_expires": 28800,
    "refresh_expires_at": "2023-02-02T05:52:51.238Z",
    "account_id": "5bd3a61d0e6846d6b0cd1bd3a00932ff",
    "client_id": "ec684b8c687f479fadea3cb2ad83f5c6",
    "internal_client": true,
    "client_service": "a5289801b5584029a35f1af1e49fe718",
    "lastPasswordValidation": "2023-02-01T21:52:51.234Z",
    "displayName": "lele test",
    "app": "a5289801b5584029a35f1af1e49fe718",
    "in_app_id": "5bd3a61d0e6846d6b0cd1bd3a00932ff",
    "product_id": "a5289801b5584029a35f1af1e49fe718",
    "application_id": "fghi4567r6GVwxCWciWCuyDCnYIxmuSF"
  }
}
```

_Example Response (Headless)_

```json
{
  "accountInfo": {
    "id": "e4ea869b3d6841f6ab2346e9b5e72648",
    "failedLoginAttempts": 0,
    "numberOfDisplayNameChanges": 0,
    "ageGroup": "UNKNOWN",
    "headless": true,
    "country": "DE",
    "preferredLanguage": "en",
    "canUpdateDisplayName": true,
    "tfaEnabled": false,
    "emailVerified": false,
    "minorVerified": false,
    "minorExpected": false,
    "minorStatus": "UNKNOWN",
    "cabinedMode": false,
    "hasHashedEmail": false
  },
  "internalAuthKey": "f048e0700a604714b0a2b117320c5cab",
  "deviceAuth": {
    "deviceId": "69a53380d32d45298eabe1a4ac2fe3ea",
    "accountId": "e4ea869b3d6841f6ab2346e9b5e72648",
    "secret": "ZKL5YKEJCKRS4QKMIRNCKLOMXPMZFKNA",
    "userAgent": "PostmanRuntime/7.30.1",
    "created": {
      "location": "Berlin, Germany",
      "ipAddress": "192.168.56.101",
      "dateTime": "2023-02-01T21:48:55.557Z"
    }
  },
  "oauthSession": {
    "access_token": "ddc4c08078cb44e0992ebc002d159d90",
    "expires_in": 7200,
    "expires_at": "2023-02-01T23:48:55.583Z",
    "token_type": "bearer",
    "refresh_token": "b2130fb18ccf4ad3a0b9c26e2274ebcc",
    "refresh_expires": 28800,
    "refresh_expires_at": "2023-02-02T05:48:55.586Z",
    "account_id": "e4ea869b3d6841f6ab2346e9b5e72648",
    "client_id": "ec684b8c687f479fadea3cb2ad83f5c6",
    "internal_client": true,
    "client_service": "a5289801b5584029a35f1af1e49fe718",
    "ext_auth_id": "f4a1d2759e1e4fcc9bce50a6c671c47c:$2a$04$cyxY5E/9eqvP4q/9Dr6KguS3aweDLwD3pU2n88tUk7ifpRba/nv4W",
    "app": "a5289801b5584029a35f1af1e49fe718",
    "in_app_id": "e4ea869b3d6841f6ab2346e9b5e72648",
    "product_id": "a5289801b5584029a35f1af1e49fe718",
    "application_id": "fghi4567r6GVwxCWciWCuyDCnYIxmuSF"
  }
}
```
