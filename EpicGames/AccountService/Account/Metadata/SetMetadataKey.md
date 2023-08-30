## Account Service - Set Metadata Key

URL: https://account-public-service-prod.ol.epicgames.com/account/api/accounts/:accountId/metadata \
Method: POST \
Auth Required: Yes (`account:accounts:{accountId}:metadata:{key} CREATE`)

```json
{
  "key": "LAUNCHER_SSO_OFF",
  "value": "true"
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`key`: The Metadata `key` to Set <br/>
`value`: The Metadata Value of the `key`

---

_Example Response_: Status 204
