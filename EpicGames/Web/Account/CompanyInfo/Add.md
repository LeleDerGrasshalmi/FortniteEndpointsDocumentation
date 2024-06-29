## Account Web - CompanyInfo: Add

URL: https://www.epicgames.com/account/v2/company-info/add \
Method: POST \
Auth Required: Yes

```json
{
  "name": "",
  "companyVatNumber": "",
  "address": {
    "country": "",
    "city": "",
    "postalCode": "",
    "line1": "",
    "line2": "",
    "region": ""
  },
  "flow_id": "account_management_prod",
  "flow_name": "",
  "solve_token": ""
}
```

## Parameters

`name`: Name of company <br/>
`companyVatNumber`: Vat Number of company <br/>
`flow_id`: Leave like that <br/>
`flow_name`: Leave like that <br/>
`solve_token`: Leave like that (Not used here, but this would be the captcha token)

---

_Example Response_

```json
{
    "success": true,
    "data": {
        "name": "krowe",
        "companyVatNumber": "AU12345678901",
        "address": {
            "country": "AU",
            "region": "hello",
            "city": "world",
            "postalCode": "0000",
            "line1": "some place on earth",
            "line2": ""
        },
        "companyVatNumberVerifiedResult": "VALID",
        "isValidCompany": true
    },
    "errorCode": null
}
```