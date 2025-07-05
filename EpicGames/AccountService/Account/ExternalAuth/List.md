## アカウントサービス-外部認証のセッションリスト

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId/externalAuths \
Method: GET \
Auth Required: Yes (`account:public:account:externalAuths READ`)

---

__レスポンスの例__

```json
[
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
]
```
