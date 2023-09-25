## Account Web - Personal: Update

URL: https://www.epicgames.com/account/v2/ajaxUpdate \
Method: POST \
Auth Required: Yes

```
country:au
flow_id:account_management_prod
flow_name:
solve_token:
```

## Headers

`Content-Type`: application/x-www-form-urlencoded

## Parameters

`param`: The Param you want to modify gotten from [here](EpicGames/Web/Account/Personal/Info.md) eg. firstName: krowe <br/>
`country`: Put the Country your account is set to <br/>
`flow_id`: Leave like that <br/>
`flow_name`: Leave like that <br/>
`solve_token`: Leave like that (Not sued here, but this would be the captcha token)
---

_Example Response_

```json
{
    "isSuccess": true,
    "country": "AU",
    "isCountryLocked": true,
    "countryChanged": false,
    "showPaymentsTab": true,
  "userInfo": {
    "id": {
      "value": "94b1569506b04f9f8557af611e8c5e47"
    },
    "displayName": {
      "value": "lele stw moment"
    },
    "firstName": {
      "value": "m***e"
    },
    "name": {
      "value": "m***e"
    },
    "email": {
      "value": "m***t@gmail.com"
    },
    "country": {
      "value": "AU"
    },
    "lastName": {
      "value": "m***m"
    },
    "preferredLanguage": {
      "value": "en"
    },
    "lastDisplayNameChange": {
      "value": "2022-12-16T20:27:19.812Z"
    },
    "canUpdateDisplayName": {
      "value": true
    },
    "tfaEnabled": {
      "value": true
    },
    "emailVerified": {
      "value": true
    },
    "cabinedMode": {
      "value": false
    },
    "hasHashedEmail": {
      "value": false
    },
    "phoneNumber": {
      "value": ""
    },
    "line1": {
      "value": ""
    },
    "line2": {
      "value": ""
    },
    "city": {
      "value": ""
    },
    "region": {
      "value": ""
    },
    "bill-pcode": {
      "value": ""
    },
    "postalCode": {
      "value": ""
    },
    "defaultAddress": {
      "value": true
    }
  }
}
```
