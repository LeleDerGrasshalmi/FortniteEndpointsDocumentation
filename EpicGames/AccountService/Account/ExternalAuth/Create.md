## アカウント認証-外部認証

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId/externalAuths \
メソッド: POST \
認証の有無: Yes (`account:public:account:externalAuths CREATE`)

```json
{
  "authType": "",
  "externalAuthToken": ""
}
```

## パラメータ

`authType`: [External Auth Readme](./README.md) と [External Auth Grant Type](../../Authentication/GrantTypes/external_auth.md#body) のドキュメントを参照してください。
`externalAuthToken`:外部プロバイダーが発行します。詳細は [こちら](../../Authentication/GrantTypes/external_auth.md#body) を参照してください。
---

__レスポンス例__

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
