## Account Service - Auth: External Auth Info

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId/externalAuths/:externalAuthType \
Method: GET \
Auth Required: Yes (`account:public:account:externalAuths READ`)

## Path Parameters

`externalAuthType`: See via [External Auth Readme](./README.md)

---

_Example Response_

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
