# Get Tax Record

URL: https://sac.epicgames.com/api/v1/get-tax-record \
Method: GET \
Auth Required: Yes

---

_Example Response_

```json
{
  "data": {
    "identityId": "0d2ccb730f2f4fac82d04bb7bb8d2d80",
    "profileType": "Individual",
    "firstName": "M***h",
    "lastName": "M***h",
    "legalName": "M***h",
    "email": "m***h@example.com",
    "phoneNumber": "****0000",
    "taxVerified": true,
    "taxStatus": "ValidatedTaxInfo",
    "taxTreatyCountryCode": "DE",
    "addressLine1": "M***0",
    "addressCity": "M***h",
    "addressState": "Mh",
    "addressCountryCode": "DE",
    "addressPostCode": "0***0",
    "mailingAddressDifferent": false,
    "mailingAddressLine1": "M***0",
    "mailingAddressCity": "M***h",
    "mailingAddressState": "M***h",
    "mailingAddressCountryCode": "D***E",
    "mailingAddressPostCode": "0***0",
    "guardianFirstName": "M***h",
    "guardianLastName": "M***h",
    "guardianEmail": "m***h@example.de",
    "recordIdentityKey": true,
    "emailStatus": "SENT",
    "lastEmailSentTime": "2022-09-15T19:10:38.927+0000",
    "emailSentCount": 1,
    "paymentHandler": "3rd-party",
    "createdAt": "2022-09-14T16:24:40.554Z",
    "usperson": false,
    "individual": true,
    "organizationEntity": false
  },
  "success": true
}
```
