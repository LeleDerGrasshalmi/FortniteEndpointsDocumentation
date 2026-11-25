## Library Service - List Collections

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/collection/account/:accountId <br/>
Method: GET <br/>
Auth Required: Yes (`library:public:{accountId}:collection READ`)

## Path Parameters

`accountId`: Your Account Id

---

*Example Response*

```json
{
  "collections": [
    {
      "collectionId": "EGS_STATIC_FAV_COLLECTION",
      "name": "Favorites",
      "libraryItemContentVersion": 1
    },
    {
      "collectionId": "55d39f5c-2253-47da-9224-cf45daec27c2",
      "name": "Hi GitHub, it's Lele",
      "libraryItemContentVersion": 5
    }
  ]
}
```
