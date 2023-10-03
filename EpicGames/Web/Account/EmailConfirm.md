## Account Web - Email: Confirm

URL: https://www.epicgames.com/account/v2/api/email/confirm \
Method: POST \
Auth Required: Yes

```json
{
    "email": "lele@example.com",
    "flow_id": "account_management_prod",
    "flow_name": "",
    "solve_token": ""
}
```

## Parameters

`email`: Your email <br/>
`flow_id`: Leave like that <br/>
`flow_name`: Leave like that <br/>
`solve_token`: Leave like that (Not used here, but this would be the captcha token)

---

_Example Response_

```json
{
    "confirmed": true
}
```
