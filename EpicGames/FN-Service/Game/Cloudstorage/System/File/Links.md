## FN Service - Cloudstorage: System File Links

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/cloudstorage/system/:uniqueFilename/links \
Method: GET \
Auth Required: Yes (`fortnite:cloudstorage:system:{uniqueFilename} READ`)

## Path Parameters

`uniqueFilename`: the `uniqueFilename` from the List

---

_Example Response_

```json
{
  "readLink": "https://d9hrb6l2qyimt.cloudfront.net/xxxxxxxxxxxx/yyyyyyyyyyyyyy/zzzzzzzzz",
  "writeLink": ""
}
```
