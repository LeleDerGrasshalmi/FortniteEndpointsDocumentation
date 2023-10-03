## Account Web - Authorized Apps: Remove App Consent

URL: https://www.epicgames.com/account/v2/authorized-apps/application/:applicationId \
Method: DELETE \
Auth Required: Yes

```json
{
  "flow_id": "account_management_prod",
  "flow_name": "",
  "solve_token": ""
}
```

## Path Parameters

`applicationId`: The Application Id, from [The "applications" List](./Apps.md)

## Parameters

`flow_id`: Leave like that <br/>
`flow_name`: Leave like that <br/>
`solve_token`: Leave like that (Not used here, but this would be the captcha token)

---

_Example Response_

```json
{
  "success": true,
  "data": {
    "applicationId": "fghi4567ENLQNc9eFlre6btvQVrxoCQh"
  }
}
```
