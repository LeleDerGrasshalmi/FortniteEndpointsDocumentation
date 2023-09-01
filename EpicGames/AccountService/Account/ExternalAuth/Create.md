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

`authType`: See via [External Auth Readme](./README.md) and also check the [External Auth Grant Type](../../Authentication/GrantTypes/external_auth.md#body) <br/>
`externalAuthToken`: Issued by the External Provider, check the [External Auth Grant Type](../../Authentication/GrantTypes/external_auth.md#body) for more Info

---

_Example Response (Same as from Info)_

```json
{
  "accountId": "94b1569506b04f9f8557af611e8c5e47",
  "type": "github",
  "externalAuthId": "lele oder so",
  "externalAuthIdType": "github_login",
  "externalDisplayName": "lele oder so",
  "authIds": [
    {
      "id": "lele oder so",
      "type": "github_login"
    }
  ],
  "dateAdded": "2023-05-26T16:50:52.040Z"
}
```
