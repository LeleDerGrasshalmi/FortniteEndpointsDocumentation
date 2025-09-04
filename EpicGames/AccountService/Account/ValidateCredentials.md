## Account Service - Validate Credentials

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId/validateCreds \
Method: POST \
Auth Required: Yes (`account:public:account:validateCreds READ`)
Note: Deprecated as of September 4th, 2025.

## Headers

`Content-Type`: `application/x-www-form-urlencoded`

<br/>

```
usernameOrEmail=XXX&password=YYY
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`usernameOrEmail`: Your Account `email` or `username` (The `username` is not the `displayName`!) <br/>
`password`: Your Account password (in plain text)

---

_Example Response (Valid)_

Status 204

<br/>

_Example Response (Invalid)_

Status 401

```json
{
  "errorCode": "errors.com.epicgames.account.invalid_account_credentials",
  "errorMessage": "Sorry the credentials you are using are invalid",
  "messageVars": [],
  "numericErrorCode": 18031,
  "originatingService": "com.epicgames.account.public",
  "intent": "prod"
}
```
