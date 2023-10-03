## Account Web - Security: Generate BackupCodes

URL: https://www.epicgames.com/account/v2/security/ajaxGenerateBackupCodes \
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
`solve_token`: Leave like that (Not used here, but this would be the captcha token)

---

_Example Response_

```json
{
  "isSuccess": true,
  "backupCodes": [
    {
      "code": "XXXXXXXX",
      "used": false
    },
    {
      "code": "XXXXXXXX",
      "used": false
    },
    {
      "code": "XXXXXXXX",
      "used": false
    },
    {
      "code": "XXXXXXXX",
      "used": false
    },
    {
      "code": "XXXXXXXX",
      "used": false
    },
    {
      "code": "XXXXXXXX",
      "used": false
    },
    {
      "code": "XXXXXXXX",
      "used": false
    },
    {
      "code": "XXXXXXXX",
      "used": false
    },
    {
      "code": "XXXXXXXX",
      "used": false
    },
    {
      "code": "XXXXXXXX",
      "used": false
    }
  ],
  "generatedAt": "2023-09-22T21:51:15.736Z"
}
```
