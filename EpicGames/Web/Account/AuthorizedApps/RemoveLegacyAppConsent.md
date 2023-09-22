## Account Web - Authorized Apps: Remove Legacy App Consent

URL: https://www.epicgames.com/account/v2/authorized-apps/application/legacy/:applicationId \
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

`applicationId`: The Application Id, from [The "legacyApplications" List](./Apps.md)

## Parameters

`flow_id`: Leave like that <br/>
`flow_name`: Leave like that <br/>
`solve_token`: Leave like that (Not sued here, but this would be the captcha token)

---

_Example Response_

```json
{
  "isSuccess": true
}
```
