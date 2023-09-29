## Account Web - Content Controls: Email Reset

URL: https://www.epicgames.com/account/v2/content-controls/send-pin-reset-email \
Method: POST \
Auth Required: Yes

```json
{
    "flow_id": "account_management_prod",
    "flow_name": "",
    "solve_token": ""
}
```

## Parameters

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