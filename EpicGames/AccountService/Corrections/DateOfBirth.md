## Account Service - Corrections: Date of Birth

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/corrections/dateOfBirth <br/>
Method: PUT <br/>
Auth Required: Yes (client_credentials of the client you are trying to authenticate with)

```json
{
  "continuation": "",
  "dateOfBirth": ""
}
```

## Parameters

`continuation`: From the [Error Response](./README.md) <br/>
`dateOfBirth`: Format is `YYYY-MM-DD`

---

*Example Response Status: 204 (No Content)*
