## Emerald Service - Upload: Complete

URL: https://emerald-service-live.ecosec.on.epicgames.com/emerald/v1/upload/complete <br/>
Method: POST <br/>
Auth Required: Yes (`emerald:upload CREATE`)

```json
{
  "token": "VjF7ImMiOiJt...NvcmRpbmcuYmluIn1dfQ=="
}
```

## Parameters

`token`: The Token received by the [init response](./Init.md)

---

*Example Response (success)*: Status 204

*Example Response (already uploaded)*

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
