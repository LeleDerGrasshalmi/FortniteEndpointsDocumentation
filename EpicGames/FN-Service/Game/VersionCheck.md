## FN バージョンチェック

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/v2/versioncheck/:platform \
メソッド: GET \
認証の有無: Yes (No special permission required)

## パスパラメータ

`platform`: プラットフォーム（例:Windows)

## クエリパラメータ

`version`: バージョンID(例：++Fortnite+Release-30.40-CL-35235494-Windows)


---

__レスポンスの例__

```js
{
    "type": "NO_UPDATE" // Could be one of these depending on version state: NO_UPDATE, NOT_ENABLED, SOFT_UPDATE, HARD_UPDATE, APP_REDIRECT
}
```

__レスポンスの例__

```js
{
    "type": "APP_REDIRECT",
    "appRedirect": "FortniteDevTesting"
}
```
