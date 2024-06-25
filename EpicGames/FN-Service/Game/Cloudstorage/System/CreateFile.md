## FN Service - Cloudstorage: Create System File

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/cloudstorage/system \
Method: POST \
Auth Required: Yes (`fortnite:cloudstorage:system CREATE`)

File Content (Binary) - **File-Body**

## Query Parameters

`filename`: The filename of the file to create

---

<br/>

_Example Response (No Perm)_

```json
{
  "errorCode": "errors.com.epicgames.common.missing_permission",
  "errorMessage": "Sorry your login does not posses the permissions 'fortnite:cloudstorage:system CREATE' needed to perform the requested operation",
  "messageVars": ["fortnite:cloudstorage:system", "CREATE"],
  "numericErrorCode": 1023,
  "originatingService": "fortnite",
  "intent": "prod-live"
}
```
