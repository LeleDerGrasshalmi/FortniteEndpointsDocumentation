## Account Service - Validate Credentials

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId/validateCreds <br/>
Method: POST <br/>
Auth Required: Yes (`account:public:account:validateCreds READ`)

## Headers

`Content-Type`: `application/x-www-form-urlencoded`

<br/>

```text
usernameOrEmail=XXX&password=YYY
```

Note: Deprecated as of September 4th, 2025.

## Path Parameters

`accountId`: Your Account Id

## Parameters

`usernameOrEmail`: Your Account `email` or `username` (The `username` is not the `displayName`!) <br/>
`password`: Your Account password (in plain text)

---

*Example Response (Valid)*

Status 204

<br/>

*Example Response (Invalid)*

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
