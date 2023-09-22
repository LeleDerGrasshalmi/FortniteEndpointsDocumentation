## Account Web - Notifications: Change Preferences

URL: https://www.epicgames.com/account/v2/api/notifications \
Method: PUT \
Auth Required: Yes

```json
{
  "settings": {
    "email": false,
    "email:egs:wishlist": false,
    "email:egs:updates": false,
    "email:fortnite": false,
    "email:fallguys": false,
    "email:rocketleague": false,
    "email:survey": false,
    "email:creatoreco:creationtools": false,
    "email:creatoreco:creationeco": false
  },
  "flow_id": "account_management_prod",
  "flow_name": "",
  "solve_token": ""
}
```

## Parameters

`settings`: The Email Preferences for the certain Setting <br/>
`flow_id`: Leave like that <br/>
`flow_name`: Leave like that <br/>
`solve_token`: Leave like that (Not sued here, but this would be the captcha token)

---

_Example Response_

```json
{
  "success": true
}
```
