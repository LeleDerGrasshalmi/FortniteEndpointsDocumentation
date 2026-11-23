## FN Service - Request Entitlement Access

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/storeaccess/v1/request_access/:accountId <br/>
Method: POST <br/>
Auth Required: Yes (Fortnite Account Auth)

## Path Parameters

`accountId`: Your Account Id

---

*Example Response (Received Entitlement)*

`Status 204`

*Example Response (Has Entitlement)*

```json
{
  "errorCode": "errors.com.epicgames.bad_request",
  "errorMessage": "Client requested access grant but already has the requested access entitlement",
  "numericErrorCode": 1001,
  "originatingService": "fortnite",
  "intent": "prod-live"
}
```
