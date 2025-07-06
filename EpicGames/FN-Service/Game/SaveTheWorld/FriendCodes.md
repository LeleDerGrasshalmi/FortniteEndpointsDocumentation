# 世界を救え。フレンドコード

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/game/v2/friendcodes/:accountId/:codeType \
メソッド: GET \
認証の有無: Yes (`fortnite:profile:{accountId}:friendcodes ALL`)

## パスパラメータ

`accountId`: アカウントID <br/>
`codeType`: `epic` または`xbox`

---

__レスポンスの例__

```json
[
  {
    "codeId": "WD3TC352GE84SCLPEXMA",
    "codeType": "CodeToken:mobileinvite",
    "dateCreated": "2018-03-27T16:54:41.385Z"
  },
  {
    "codeId": "WD3TC352GE84SCLPEXMA",
    "codeType": "CodeToken:founderfriendinvite",
    "dateCreated": "2018-03-27T16:54:41.385Z"
  }
]
```
