## EGS Platform Service - Account: Parental Controls - Verify Pin

URL: https://egs-platform-service.store.epicgames.com/api/v1/private/egs/account/content-controls/verify-pin \
Method: POST \
Auth Required: Yes

```json
{
  "pin": "000000"
}
```

## Parameters

`pin`: Your parental verification pin

---

_Example Response (correct pin)_

```json
{
  "status": "Success"
}
```

_Example Response (invalid pin)_

```json
{
  "errorMessage": "Invalid pin"
}
```
