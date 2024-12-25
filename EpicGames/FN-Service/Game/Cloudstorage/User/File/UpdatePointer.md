## FN Service - Cloudstorage: Update Pointer (Migrate to DSS)

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/cloudstorage/user/:accountId/:uniqueFilename/updatePointer \
Method: POST \
Auth Required: Yes (`fortnite:cloudstorage:user:{accountId}:{uniqueFilename} UPDATE`)

```json
{
  "moduleName": "DSS",
  "pointer": "cloudstorage/Live/user/94b1569506b04f9f8557af611e8c5e47/a.sav",
  "fileHash": "0000000000000000000000000000000000000000",
  "length": 0
}
```

## Path Parameters

`accountId`: Your Account Id <br/>
`uniqueFilename`: The `uniqueFilename` from list, e.g. `ClientSettings.sav` or `ClientSettingsPS5.sav`

## Parameters

`moduleName`: Only `DSS` is known to support pointer updates <br/>
`pointer`: Pointer reference within the module <br/>
`fileHash`: File SHA1 Hash <br/>
`length`: File Byte Count

## Query Parameters

`shouldMigrate`: Boolean, that is used for migrations

---

_Example Response (success)_

```json
{
  "uniqueFilename": "ClientSettingsPS4.sav",
  "filename": "ClientSettingsPS4.sav",
  "hash": "0000000000000000000000000000000000000000",
  "hash256": "",
  "length": 0,
  "contentType": "binary/octet-stream",
  "uploaded": "2024-12-25T16:10:39.061Z",
  "storageType": "DSS",
  "storageIds": {
    "DSS": "cloudstorage/Live/user/94b1569506b04f9f8557af611e8c5e47/a.sav"
  },
  "metadata": {},
  "accountId": "94b1569506b04f9f8557af611e8c5e47"
}
```

_Example Response (unsupported module)_

```json
{
  "errorCode": "errors.com.epicgames.cloudstorage.invalid_user_storage_data",
  "errorMessage": "external pointer updates are not supported for the given provider",
  "messageVars": [],
  "numericErrorCode": 12016,
  "originatingService": "fortnite",
  "intent": "prod-live"
}
```

_Example Response (mismatch)_

```json
{
  "errorCode": "errors.com.epicgames.cloudstorage.user_file_move_failed",
  "errorMessage": "migrations are not enabled and given hash '0000000000000000000000000000000000000000', length 0 does not match stored hash '0000000000000000000000000000000000000000', length 0 for file 'ClientSettingsPS4.sav'",
  "messageVars": [
    "0000000000000000000000000000000000000000",
    "0",
    "0000000000000000000000000000000000000000",
    "0",
    "ClientSettingsPS4.sav"
  ],
  "numericErrorCode": 12011,
  "originatingService": "fortnite",
  "intent": "prod-live"
}
```
