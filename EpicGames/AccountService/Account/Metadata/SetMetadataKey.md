## メタデータキーの設定API

URL: https://account-public-service-prod.ol.epicgames.com/account/api/accounts/:accountId/metadata \
メソッド: POST \
認証の有無: Yes (`account:accounts:{accountId}:metadata:{key} CREATE`)

```json
{
  "key": "LAUNCHER_SSO_OFF",
  "value": "true"
}
```

## パスパラメータ

`accountId`: アカウントID

## パラメータ

`key`:  `yourkey`  <br/>
`value`:  `yourkey`

---

__レスポンスの例__：status204
