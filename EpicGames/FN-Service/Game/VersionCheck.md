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

```json
{
    "type": "NO_UPDATE" // Could be one of these depending on version state: NO_UPDATE, NOT_ENABLED, SOFT_UPDATE, HARD_UPDATE, APP_REDIRECT
}
```

