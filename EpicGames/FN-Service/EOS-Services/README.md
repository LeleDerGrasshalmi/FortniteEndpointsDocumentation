# Epic Online Servicesの認証

これらのAPIはEOS Connect認証を必要とします。トークンの取得方法の例を以下に示します。
したがって、リクエストにリストされている権限はポリシー権限であり、クライアント権限ではありません（これがEOSの仕組みです）。

---

URL: https://api.epicgames.dev/auth/v1/oauth/token \
メソッド: POST \
認証の有無: Yes (`ユーザー名`がクライアントID、`パスワード`がクライアントシークレットである基本認証)

## ヘッダー

`Content-Type`: `application/x-www-form-urlencoded`

## パラメータ

`grant_type`: `external_auth` <br/>
`external_auth_type`: `epicgames_access_token` <br/>
`external_auth_token`:通常のアクセストークン <br/>
`deployment_id`: 環境変数からのデプロイメントID <br/>
`nonce`: ランダムなノンス文字列

---

__レスポンスの例__

```json
{
  "access_token": "REDACTED",
  "token_type": "bearer",
  "expires_at": "2024-11-16T19:02:54.328Z",
  "nonce": "_",
  "features": [
    "AntiCheat",
    "Connect",
    "ContentService",
    "Ecom",
    "Inventories",
    "LockerService",
    "Matchmaking Service"
  ],
  "organization_id": "o-aa83a0a9bc45e98c80c1b1c9d92e9e",
  "product_id": "prod-fn",
  "sandbox_id": "fn",
  "deployment_id": "62a9473a2dca46b29ccf17577fcf42d7",
  "organization_user_id": "00012606a6424b879ad5ef5978bfe879",
  "product_user_id": "00023ceb23764ee6a3199c9f4a387a9e",
  "product_user_id_created": false,
  "id_token": "REDACTED",
  "expires_in": 3599
}
```

---

ゲームから送信されるプレーンなhttpリクエストの例

```http
POST https://api.epicgames.dev/auth/v1/oauth/token HTTP/1.1
Host: api.epicgames.dev
Accept-Encoding: identity
Content-Type: application/x-www-form-urlencoded
Accept: application/json
Authorization: Basic ZWM2ODRiOGM2ODdmNDc5ZmFkZWEzY2IyYWQ4M2Y1YzY6ZTFmMzFjMjExZjI4NDEzMTg2MjYyZDM3YTEzZmM4NGQ=
X-Epic-Correlation-ID: EOS-REDACTED
User-Agent: EOS-SDK/1.16.3000-33300249 (Windows/10.0.19041.4165.64bit) Fortnite/++Fortnite+Release-30.00-CL-33962396
X-EOS-Version: 1.16.3000-33300249

grant_type=external_auth&external_auth_type=epicgames_access_token&external_auth_token=REDACTED&deployment_id=62a9473a2dca46b29ccf17577fcf42d7&nonce=REDACTED
```
