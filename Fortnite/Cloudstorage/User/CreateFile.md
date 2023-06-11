## Fortnite - Cloudstorage: Create User File

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/cloudstorage/user \
Method: POST \
Auth Required: Yes (`fortnite:cloudstorage:user:{accountId}:{filename} CREATE`)

File Content (Binary) - **File-Body**

## Query Parameters

`filename`: The filename of the file to create

---

_Example Response (Created)_

`ClientSettingsPS4.sav` (Unique Filename)

<br/>

_Example Response (Already Exists)_

```json
{
  "errorCode": "errors.com.epicgames.common.mongo_write_error",
  "errorMessage": "Sorry, there was an error writing to the database.",
  "numericErrorCode": 1060,
  "originatingService": "fortnite",
  "intent": "prod-live"
}
```
