## FN Service - Cloudstorage: User Files

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/cloudstorage/user/:accountId \
Method: GET \
Auth Required: Yes (`fortnite:cloudstorage:user:{accountId} READ`)

## Path Parameters

`accountId`: Your Account Id

---

_Example Response_

```json
[
  {
    "uniqueFilename": "ClientSettings.Sav",
    "filename": "ClientSettings.Sav",
    "hash": "ecf9b6ba7a494358b7bdf36fb70d423b013a4f4e",
    "hash256": "5867145b3536492362f511ebb59a56acf976d28b6723a0727789487814b857bc",
    "length": 15462,
    "contentType": "application/octet-stream",
    "uploaded": "2023-05-17T15:57:43.883Z",
    "storageType": "S3",
    "storageIds": {},
    "metadata": {
      "isHotfix": {
        "empty": true,
        "present": false
      }
    },
    "accountId": "94b1569506b04f9f8557af611e8c5e47"
  }
]
```
