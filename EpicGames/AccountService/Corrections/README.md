# Error Response

When an corrective action is required, you will get such an error response when authenticating.

```json
{
  "errorCode": "errors.com.epicgames.oauth.corrective_action_required",
  "errorMessage": "Corrective action is required to continue.",
  "messageVars": [],
  "numericErrorCode": 18206,
  "originatingService": "com.epicgames.account.public",
  "intent": "prod",
  "continuation": "00000000000000000000000000000000",
  "continuationUrl": "https://epicgames.com/continue/00000000",
  "correctiveAction": "DATE_OF_BIRTH"
}
```
