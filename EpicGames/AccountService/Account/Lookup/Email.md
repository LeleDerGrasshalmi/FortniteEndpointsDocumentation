## アカウントサービス-メールアドレスによる検索

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/email/:email \
メソッド: GET \
認証の有無: Yes (~~`account:public:account:byEmail`~~ `account:public:account:lookup:email READ`)

## パスパラメータ

`email`: メールアドレス

---

__レスポンスの例__

```json
{
  "id": "94b1569506b04f9f8557af611e8c5e47",
  "displayName": "lele stw moment",
  "externalAuths": {}
}
```

> **レート制限** :3回/600秒

このAPIは未成年者などのデータ保護のため、2023 年 1 月 14 日 をもって廃止されました。
