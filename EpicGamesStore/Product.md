## ストアページ

URL: https://store-content.ak.epicgames.com/api/:locale/content/products/:product \
メソッド: GET \
認証の有無: No

## パスパラメータ

`en-US`: ローカル言語,(例:`ja-JP`) <br/>
`product`:製品スラッグ。例: `fortnite`

__レスポンスの例（短縮版）__

```json
{
  "disableNewAddons": false,
  "modMarketplaceEnabled": false,
  "_title": "fortnite",
  "regionBlock": "IOS",
  "_noIndex": false,
  "productName": "Fortnite",
  "namespace": "fn",
  "reviewOptOut": false,
  "_urlPattern": "/productv2/fortnite",
  "_slug": "fortnite",
  "_activeDate": "2018-10-17T13:50:57.250Z",
  "lastModified": "2022-01-19T18:21:00.756Z",
  "_locale": "en-US",
  "_id": "7b47179d-a281-47ae-a2e0-8432697d4824",
  "_templateName": "productNamespace",
  "pages": [
    {
      "namespace": "fn",
      "reviewOptOut": false,
      "_urlPattern": "/productv2/fortnite/home",
      "_slug": "home",
      "_activeDate": "2022-07-21T13:00:00.000Z",
      "lastModified": "2023-06-13T23:29:52.331Z",
      "_locale": "en-US",
      "_id": "af8e309a-019d-42dd-899c-a05908ba4be5",
      "_templateName": "productDetail",
      "item": {
        "catalogId": "4fe75bbc5a674f4f9b356b5c90567da5",
        "appName": "Fortnite",
        "namespace": "fn",
        "hasItem": true
      },
      "overwriteMapping": false,
      "ageGate": {
        "hasAgeGate": false
      },
      "_images_": [
        "https://cdn2.unrealengine.com/landscape-2560x1440-46bf2efbac01.jpg"
      ]
    }
  ]
}
```
