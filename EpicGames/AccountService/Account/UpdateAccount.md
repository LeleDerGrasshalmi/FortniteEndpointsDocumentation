## Account Service - Update Account

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId \
Method: PUT \
Auth Required: Yes (`account:public:account UPDATE`, some need `account:public:account:sensitive UPDATE`)

```json
{
  "name": "_",
  "lastName": "_",
  "preferredLanguage": "de",
  "displayName": "lele stw moment",
  "phoneNumber": "0123456789",
  "company": "Lele Exploits",
  "email": "lele@example.com",
  "username": "lele",
  "password": "hey123!"
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`name`: Optional, Your new Firstname <br/>
`lastName`: Optional, Your new Lastname <br/>
`preferredLanguage`: Optional, Your new Preferred Language <br/>
`displayName`: Optional, Your new Display Name <br/>
`phoneNumber`: Optional, Your new Phone-Number <br/>
`company`: Optional, Your new Company <br/>
`email`: Optional, Your new Email `[*]` <br/>
`username`: Optional, Your new Username (could be used instead of an email back then) `[*]` <br/>
`password`: Optional, Your new Password `[*]` <br/>

`[*]` - Requires the sensitive Permission

---

_Example Response_

```json
{
  "accountInfo": {
    "id": "94b1569506b04f9f8557af611e8c5e47",
    "displayName": "lele stw moment",
    "email": "lele@example.com",
    "failedLoginAttempts": 0,
    "lastLogin": "2023-05-02T16:51:59.221Z",
    "numberOfDisplayNameChanges": 1,
    "dateOfBirth": "2000-01-03",
    "ageGroup": "ADULT",
    "headless": false,
    "country": "DE",
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
    "cabinedMode": false,
    "hasHashedEmail": false
  }
}
```
