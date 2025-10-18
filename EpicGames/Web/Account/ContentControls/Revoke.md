## Account Web - Content Controls: Revoke

URL: https://www.epicgames.com/account/v2/content-controls/third-parties/revoke \
Method: POST \
Auth Required: Yes

```json
{
    "pin": "012345"
}
```

## Parameters

`pin`: The Parental Code (6 Numeric Chars) 

---

_Example Response (Valid)_

```json
{
    "success": true,
    "data": {
        "showThirdParties": false,
        "thirdPartiesEnabled": false,
        "connectedAppsCtn": 0
    }
}
```