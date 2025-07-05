## 購入証明書

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/receipts/v1/account/:accountId/receipts \
メソッド: GET \
認証の有無: Yes (`fortnite:profile:{accountId}:receipts ALL`)

# パスパラメータ
`accountId`: アカウントID

---

__レスポンスの例__

```json
[
  {
    "appStore": "EpicPurchasingService",
    "appStoreId": "0d9a0d1012564f0280ad4ebf3e1e5fce",
    "receiptId": "62f9cfd5447e47bcb09f2260f332cfef",
    "receiptInfo": "ENTITLEMENT"
  }
]
```
