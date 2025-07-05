## アカウントサービス-外部ディスプレイネームの一括検索

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/lookup/externalDisplayName \
メソッド: POST \
認証の有無: Yes (`account:public:account:lookup:externalDisplayName:{externalAuthType} READ`)

```json
{
  "authType": "xbl",
  "displayNames": ["jemcer"]
}
```

## パラメータ

`authType`: [こちら](../../ExternalAuth/README.md) を参照してください。<br/>
`displayNames`:  表示名、大文字と小文字を区別[**リクエストあたり最大100**]

---

__レスポンス例__

```json
{
  "jemcer": [
    {
      "accountId": "bec13864ce1d44148e04cb82401c4257",
      "type": "xbl",
      "externalAuthIdType": "xuid",
      "externalDisplayName": "jemcer"
    }
  ]
}
```
