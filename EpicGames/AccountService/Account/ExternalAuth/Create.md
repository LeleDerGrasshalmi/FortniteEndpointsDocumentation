## Account Service - Auth: Create External Auth

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId/externalAuths <br/>
Method: POST <br/>
Auth Required: Yes (`account:public:account:externalAuths CREATE`)

```json
{
  "authType": "",
  "externalAuthToken": ""
}
```

## Path Parameters

`accountId`: The account ID.

## Parameters

`authType`: See via [External Auth Readme](./README.md) and also check the [External Auth Grant Type](../../Authentication/GrantTypes/external_auth.md#body) <br/>
`externalAuthToken`: Issued by the External Provider, check the [External Auth Grant Type](../../Authentication/GrantTypes/external_auth.md#body) for more Info

---

*Example Response (Same as from Info)*

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
