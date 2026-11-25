## EGS Platform Service - Account: Parental Controls - Verify Pin

URL: https://egs-platform-service.store.epicgames.com/api/v1/private/egs/account/content-controls/verify-pin <br/>
Method: POST <br/>
Auth Required: Yes

```json
{
  "pin": "000000"
}
```

## Parameters

`pin`: Your parental verification pin

---

*Example Response (correct pin)*

```json
{
  "status": "Success"
}
```

*Example Response (invalid pin)*

```json
{
  "errorMessage": "Invalid pin"
}
```
