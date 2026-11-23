## FN Service - Client Feature Keys

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/game/v2/clientfeaturekeys/:accountId <br/>
Method: GET <br/>
Auth Required: Yes (`fortnite:profile:{accountId}:commands UPDATE`)

## Path Parameters

`accountId`: Your Account Id

---

*Example Response (None)*

```json
{
  "errorCode": "errors.com.epicgames.fortnite.invalid_featurekey_request",
  "errorMessage": "Account access tier does not include any client feature keys",
  "messageVars": [],
  "numericErrorCode": -1,
  "originatingService": "fortnite",
  "intent": "prod-live"
}
```
