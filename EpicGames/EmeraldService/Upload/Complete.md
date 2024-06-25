## Emerald Service - Upload: Complete

URL: https://emerald-service-live.ecosec.on.epicgames.com/emerald/v1/upload/complete \
Method: POST \
Auth Required: Yes (`emerald:upload CREATE`)

```json
{
  "token": "VjF7ImMiOiJt...NvcmRpbmcuYmluIn1dfQ=="
}
```

## Parameters

`token`: The Token received by the [init response](./Init.md)

---

_Example Response (success)_: Status 204

_Example Response (already uploaded)_

```json
{
  "errorCode": "errors.com.epicgames.server_error",
  "errorMessage": "An unexpected server error has occurred.",
  "numericErrorCode": 1000,
  "messageVars": ["invalid item state: UploadFinished"],
  "originatingService": "com.epicgames.emerald-service",
  "intent": "live"
}
```
