## Wex Service - Cloudstorage: System Files

URL: https://wex-public-service-live-prod.ol.epicgames.com/wex/api/cloudstorage/system \
Method: GET \
Auth Required: Yes (`wexp:cloudstorage:system READ`)

---

_Example Response (shortened)_

```json
[
  {
    "uniqueFilename": "a6b5e5b09d0b426db3616c919b2af9b0",
    "filename": "DefaultEngine.ini",
    "hash": "ac740e157b4ef5c578e76f50ee8997ffb5c9f442",
    "hash256": "ab74b8b51e673b3fa8095192e6463de35e6683fcaacf38538bd0392f6e6b9894",
    "length": 137,
    "contentType": "application/octet-stream",
    "uploaded": "2019-12-15T19:36:11.935Z",
    "storageType": "S3",
    "doNotCache": false
  }
]
```
