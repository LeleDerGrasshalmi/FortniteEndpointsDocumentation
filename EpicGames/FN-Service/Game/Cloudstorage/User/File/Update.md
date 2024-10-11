## FN Service - Cloudstorage: Update User File

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/cloudstorage/user/:accountId/:uniqueFilename \
Method: PUT \
Auth Required: Yes (`fortnite:cloudstorage:user:{accountId}:{uniqueFilename} UPDATE`)

File Content (Binary) - **File-Body**

## Path Parameters

`accountId`: Your Account Id <br/>
`uniqueFilename`: The `uniqueFilename` from list, e.g. `ClientSettings.sav` or `ClientSettingsPS5.sav`

---

_Example Response_

> If the file got created with the request, the response is the `uniqueFilename` as plain text, <br/>
> otherwhise it just returns status 200 with no content
