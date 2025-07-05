## ギフトを送る相手のステータスを確認するAPI

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/storefront/v2/gift/check_eligibility/recipient/:friendId/offer/:offerId \
メソッド: GET \
認証の有無: Yes 

# パスパラメータ

`friendId`: アカウントID<br/>
`offerId`:URLエンコードされたオファーID

---

__レスポンスの例(相手がアイテムを所有していない場合)__

```json
{
  "price": {
    "currencyType": "MtxCurrency",
    "currencySubType": "",
    "regularPrice": 200,
    "dynamicRegularPrice": 200,
    "finalPrice": 200,
    "saleExpiration": "9999-12-31T23:59:59.999Z",
    "basePrice": 200
  },
  "items": [
    {
      "templateId": "AthenaDance:eid_vectorsparkv3",
      "quantity": 1
    }
  ]
}
```
