## アカウントサービス-外部IDによる一括検索

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/lookup/externalId \
メソッド: POST \
認証の有無: Yes (`account:public:account:lookup:externalId READ`)

```json
{
  "authType": "nintendo",
  "ids": ["lp1_e7b6e8e2e07fab26"]
}
```

## パラメータ

`authType`: [こちら](../../ExternalAuth/README.md)を参照してください。 <br/>
`ids`: 外部アカウントの文字列番号です[**リクエストあたり最大100**]

---

__レスポンスの例**

```json
{
  "lp1_e7b6e8e2e07fab26": {
    "accountId": "020b5d9042174a7692f20db8e23b84d1",
    "type": "nintendo",
    "externalAuthId": "lp1_e7b6e8e2e07fab26",
    "externalAuthIdType": "nintendo_id",
    "authIds": [
      {
        "id": "lp1_e7b6e8e2e07fab26",
        "type": "nintendo_id"
      }
    ]
  }
}
```
