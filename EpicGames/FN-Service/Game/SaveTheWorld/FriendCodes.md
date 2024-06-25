## FN Service - STW Friend Codes

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/game/v2/friendcodes/:accountId/:codeType \
Method: GET \
Auth Required: Yes (`fortnite:profile:{accountId}:friendcodes ALL`)

## Path Parameters

`accountId`: Your Account Id <br/>
`codeType`: `epic` or `xbox`

---

_Example Response_

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
