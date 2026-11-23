## FN Service - Cloudstorage: Create User File

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/cloudstorage/user/:accountId <br/>
Method: POST <br/>
Auth Required: Yes (`fortnite:cloudstorage:user:{accountId}:{filename} CREATE`)

File Content (Binary) - **File-Body**

## Path Parameters

`accountId`: Your Account Id

## Query Parameters

`filename`: The filename of the file to create

---

*Example Response (Created)*

`ClientSettingsPS4.sav` (Unique Filename)

<br/>

*Example Response (Already Exists)*

```json
{
  "errorCode": "errors.com.epicgames.common.mongo_write_error",
  "errorMessage": "Sorry, there was an error writing to the database.",
  "numericErrorCode": 1060,
  "originatingService": "fortnite",
  "intent": "prod-live"
}
```
