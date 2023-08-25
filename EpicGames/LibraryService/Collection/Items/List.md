## Library Service - List Collection Items

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/collection/:collectionId/item/account/:accountId \
Method: GET \
Auth Required: Yes (`library:public:{accountId}:collection:item READ`)

## Path Parameters

`collectionId`: The Collection Id (UUIDv4) <br/>
`accountId`: Your Account Id

---

_Example Response_

```json
{
  "responseMetadata": {},
  "records": [
    {
      "sandbox": "33956bcb55d4452d8c47e16b94e294bd",
      "catalogId": "729a86a5146640a2ace9e8c595414c56",
      "artifactId": "963137e4c29d4c79a81323b8fab03a40"
    }
  ]
}
```
