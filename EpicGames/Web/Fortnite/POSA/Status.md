## Fortnite Website - POSA: Status

URL: https://fortnite.com/:locale/api/posa/code/status <br/>
Method: POST <br/>
Auth Required: Yes

```json
{
  "code": ""
}
```

## Path Parameters

`locale`: The Locale of the Response, defaults to `en-US` if invalid

## Parameters

`code`: The Code to check

---

*Example Response (Invalid Code)*

```json
{
  "errorCode": "errors.com.epicgames.posa.cardNotFound",
  "success": false
}
```
