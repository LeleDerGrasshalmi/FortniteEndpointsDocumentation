## Account Web - Content Controls: Reset

URL: https://www.epicgames.com/account/v2/content-controls/reset-pin \
Method: POST \
Auth Required: Yes

```json
{
    "pin": "012345",
    "pinConfirm": "012345",
    "newPin": "000000",
    "flow_id": "account_management_prod",
    "flow_name": "",
    "solve_token": ""
}
```

## Parameters

`pin`: The Parental Code (6 Numeric Chars) <br/>
`pinConfirm`: The Parental Code (6 Numeric Chars) <br/>
`newPin`: The New Parental Code To Set (6 Numeric Chars) <br/>
`flow_id`: Leave like that <br/>
`flow_name`: Leave like that <br/>
`solve_token`: Leave like that (Not sued here, but this would be the captcha token)

---

_Example Response (Valid)_

```json
{
    "success": true,
    "status": 200,
    "data": {
        "success": true
    }
}
```