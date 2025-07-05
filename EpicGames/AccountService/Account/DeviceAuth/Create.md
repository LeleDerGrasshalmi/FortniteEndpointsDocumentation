## アカウントサービス-デバイスの認証

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId/deviceAuth \
メソッド: POST \
認証の有無: Yes (`account:public:account:deviceAuths CREATE`)

---

_レスポンスの例_

```json
{
  "deviceId": "435b52ece6d347479531c5132e209e53",
  "accountId": "94b1569506b04f9f8557af611e8c5e47",
  "secret": "MPIPS4XUSSC766PFRG5JZZPASUTTZNAN",
  "userAgent": "",
  "created": {
    "location": "Germany",
    "ipAddress": "127.0.0.1",
    "dateTime": "2023-01-11T17:31:05.418Z"
  }
}
```
