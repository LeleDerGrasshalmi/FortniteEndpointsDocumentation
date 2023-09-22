## Account Web - Content Controls: Verify Pin

URL: https://www.epicgames.com/account/v2/content-controls/verify-pin \
Method: POST \
Auth Required: Yes

```json
{
  "pin": "012345",
  "flow_id": "account_management_prod",
  "flow_name": "",
  "solve_token": ""
}
```

## Parameters

`pin`: The Parental Code (6 Numeric Chars) <br/>
`flow_id`: Leave like that <br/>
`flow_name`: Leave like that <br/>
`solve_token`: Leave like that (Not sued here, but this would be the captcha token)

---

_Example Response (Valid)_

```json
{
  "success": true
}
```

_Example Response (Invalid)_

```json
{
  "success": false,
  "errors": {
    "pin": {
      "fieldName": "pin",
      "errorCode": "errors.com.epicgames.content_controls.invalid_pin"
    },
    "pinConfirm": null
  },
  "message": "Validation failure",
  "version": "v1"
}
```
