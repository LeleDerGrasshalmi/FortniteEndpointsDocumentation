## KWS - Send Verify Email

URL: https://api.kws.ol.epicgames.com/v1/verifications/send-email \
Method: POST \
Auth Required: Yes

```json
{
  "email": "lele@example.com",
  "location": "GB",
  "language": "en",
  "externalPayload": "{\"id\":\"123xyz\"}",
  "redirectUrlOverride": "https://your.app.redirect.com",
  "userContext": "parent"
}
```

## Parameters

`email`: Email to verify <br/>
`location`: The location code of the location where the user requiring verification resides. Must be in ISO 3166-1 alpha-2 or ISO 3166-2 format. e.g. 'US', 'GB', 'AD-07' <br/>
`language`: e.g. 'en', 'ja', 'de'. See the KWS Developer's Guide for supported languages <br/>
`externalPayload`: Optional. A payload that will be passed back via webhook notifications resulting from this request. This payload will not be processed or validated other than for type of string, with max length of 200 characters <br/>
`redirectUrlOverride`: Optional. If specified, this URL will override the post-verification flow redirect for the given product and service specified within your developer portal account <br/>
`userContext`: The user context is used when building out the user flow

---

_Example Response (insufficient permissions)_

```json
{
  "meta": {
    "requestId": "588ffe00-1eaa-11ef-ae5b-a509b44f3cee",
    "timestamp": "2024-05-30T17:30:45.088Z"
  },
  "error": {
    "statusCode": 401,
    "code": "ERR_UNAUTHORISED",
    "message": "Authentication credentials provided are not valid or missing",
    "errorCode": "unauthorised"
  }
}
```
