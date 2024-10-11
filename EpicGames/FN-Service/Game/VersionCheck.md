## FN Service - Version Check

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/v2/versioncheck/:platform \
Method: GET \
Auth Required: Yes (No special permission required)

## Path Parameters

`platform`: The platform to check (ex. Windows)

## Query Parameters

`version`: The version to check (URL-Encoded, ex. ++Fortnite+Release-30.40-CL-35235494-Windows)

---

_Example Response_

```js
{
    "type": "NO_UPDATE" // Could be one of these depending on version state: NO_UPDATE, NOT_ENABLED, SOFT_UPDATE, HARD_UPDATE, APP_REDIRECT
}
```

_Example Response (If type is `APP_REDIRECT`)_

```js
{
    "type": "APP_REDIRECT",
    "appRedirect": "FortniteDevTesting"
}
```
