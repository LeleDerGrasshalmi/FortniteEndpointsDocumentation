## Account Service - Auth: Create External Auth

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId/externalAuths \
Method: POST \
Auth Required: Yes (`account:public:account:externalAuths CREATE`)

```json
{
  "authType": "",
  "externalAuthToken": ""
}
```

## Parameters

`authType`: See via [External Auth Readme](./README.md) <br/>
`externalAuthToken`: Issued by the External Provider, check the Readme for more info
