## Fortnite Website - POSA: Status

URL: https://fortnite.com/:locale/api/posa/code/status \
Method: POST \
Auth Required: Yes

```json
{
  "code": ""
}
```

## Query Parameters

`locale`: The Locale of the Response, defaults to `en-US` if invalid

---

_Example Response (Invalid Code)_

```json
{
  "errorCode": "errors.com.epicgames.posa.cardNotFound",
  "success": false
}
```
