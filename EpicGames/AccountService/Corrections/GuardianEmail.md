## Account Service - Corrections: Guardian Email

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/corrections/guardianEmail \
Method: PUT \
Auth Required: Yes (client_credentials of the client you are trying to authenticate with)

```json
{
  "continuation": "",
  "guardianEmail": ""
}
```

## Parameters

`continuation`: From the [Error Response](./README.md) <br/>
`guardianEmail`: Email of the Guardian (Parent)

---

_Example Response Status: 204 (No Content)_
