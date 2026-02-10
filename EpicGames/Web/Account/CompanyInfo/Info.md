## Account Web - CompanyInfo: Info

URL: https://www.epicgames.com/account/v2/company-info \
Method: GET \
Auth Required: Yes

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
}
```