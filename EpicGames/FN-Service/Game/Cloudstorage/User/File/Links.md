## FN Service - Cloudstorage: User File Links

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/cloudstorage/user/:accountId/:uniqueFilename/links \
Method: GET \
Auth Required: Yes (`fortnite:cloudstorage:user:{accountId}:{uniqueFilename} CREATE`)

## Path Parameters

`accountId`: Your Account Id <br/>
`uniqueFilename`: The `uniqueFilename` from list, e.g. `ClientSettings.sav` or `ClientSettingsPS5.sav`

---

_Example Response_

_As of 19th may 2023, this is not supported on User Files, but the API itself exists, the feature is just not enabled_

```json
{
  "errorCode": "errors.com.epicgames.cloudstorage.file_storage_data_load_exception",
  "errorMessage": "no enabled DAOs were able to provide links for file 'ClientSettings.Sav'",
  "messageVars": ["ClientSettings.Sav"],
  "numericErrorCode": 12020,
  "originatingService": "fortnite",
  "intent": "prod-live"
}
```
