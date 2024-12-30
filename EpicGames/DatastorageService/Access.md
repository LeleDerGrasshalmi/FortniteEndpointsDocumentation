## FN Service - Datastorage: Access File

URL: https://datastorage-public-service-live.ol.epicgames.com/api/v1/access/fortnite/:id \
Method: GET \
Auth Required: Yes (`fortnite:cloudstorage:system READ`)

## Path Parameters

`id`: DSS id of a cloudstorage object

---

_Example Response_

```json
{
  "files": {
    "cloudstorage/Live/system/1/550d13f0917044e6876e217d24da10f8-c52c1f9246eb48ce9dade87be5a66f29": {
      "readLink": "https://d9hrb6l2qyimt.cloudfront.net/cloudstorage%2FLive%2Fsystem%2F1%2F550d13f0917044e6876e217d24da10f8-c52c1f9246eb48ce9dade87be5a66f29?Expires=1735591798&Signature=ijbtoJ8brb1UQSEcMsFCh2sOTU5MT7Dy3wWqVm9ijIBPJpN4Ju4VMEGFW7EDytBi7zlodiGEv16WwAZnWuYb~P2eNKweMDUDOe4A0fkYU-PTnKIv~gZqfBjuQi0gfDu8fxb4KMSDJbvQ9NUo5MTLtSDbYZ1pM8dPKlInGxrdOkGTNnn0NtKHdwXCS9NmTYauRk19On4YySEllLf2y6spb1~gg~Qi26KsmrdIHDjhEjyLP6-TbDGFtY~2YC2rscQS5gJ0ebXoVqTofRk8pkAJRU8TbgbYGIxXCisrVjlvMXCE6vq1RNklUn4hZHOk4p7gQrNZUcfsPzspsueT1MyP8g__&Key-Pair-Id=APKAI5CNFPJPTPYZISXQ",
      "writeLink": null,
      "hash": null,
      "lastModified": null,
      "size": 0,
      "fileLocked": false
    }
  },
  "folderThrottled": false,
  "maxFileSizeBytes": -1,
  "maxFolderSizeBytes": -1,
  "expiresAt": "2024-12-30T20:49:58.329Z"
}
```
