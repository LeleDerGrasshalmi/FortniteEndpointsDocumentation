## Account Web - Personal: Update Displayname

URL: https://www.epicgames.com/account/v2/personal/update-display-name \
Method: POST \
Auth Required: Yes

```
displayName:leledocs
flow_id:account_management_prod
flow_name:
solve_token:
```

## Headers

`Content-Type`: application/x-www-form-urlencoded

## Parameters

`displayName`: The Username you want <br/>
`flow_id`: Leave like that <br/>
`flow_name`: Leave like that <br/>
`solve_token`: Leave like that (Not used here, but this would be the captcha token)
---

_Example Response_

```json
{
    "success": true,
    "data": {
        "lastDisplayNameChange": "2024-08-07T09:22:30.873Z",
        "canUpdateDisplayName": false,
        "canUpdateDisplayNameNext": "2024-08-21T09:22:30.873Z",
        "displayName": "leledocs",
        "displayNameChanged": true
    }
}
```
