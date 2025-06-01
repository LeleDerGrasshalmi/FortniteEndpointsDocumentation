## FN Service - Request Entitlement Access

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/storeaccess/v1/request_access/:accountId \
Method: GET \
Auth Required: Yes (Fortnite Account Auth)

## Path Parameters

`accountId`: Your Account Id

---

_Example Response (Received Entitlement)_

`Status 204`

_Example Response (Has Entitlement)_

```json
{
  "errorCode": "errors.com.epicgames.bad_request",
  "errorMessage": "Client requested access grant but already has the requested access entitlement",
  "numericErrorCode": 1001,
  "originatingService": "fortnite",
  "intent": "prod-live"
}
```
