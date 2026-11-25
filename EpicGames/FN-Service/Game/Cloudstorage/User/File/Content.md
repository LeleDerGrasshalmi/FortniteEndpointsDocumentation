## FN Service - Cloudstorage: User File Content

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/cloudstorage/user/:accountId/:uniqueFilename <br/>
Method: GET <br/>
Auth Required: Yes (`fortnite:cloudstorage:user:{accountId}:{uniqueFilename} READ`)

## Path Parameters

`accountId`: Your Account Id <br/>
`uniqueFilename`: The `uniqueFilename` from list, e.g. `ClientSettings.sav` or `ClientSettingsPS5.sav`

---

*Example Response*

Returns the contents of the requested file. The format depends on the file.
