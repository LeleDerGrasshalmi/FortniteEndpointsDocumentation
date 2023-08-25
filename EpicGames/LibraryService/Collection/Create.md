## Library Service - Create Collection

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/collection/account/:accountId \
Method: POST \
Auth Required: Yes (`library:public:{accountId}:collection CREATE`)

```json
{
  "name": "Hi GitHub, this is Lele"
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`name`: The name of the new Collection

---

_Example Response_

```json
{
  "collectionId": "55d39f5c-2253-47da-9224-cf45daec27c2",
  "name": "Hi GitHub, this is Lele",
  "libraryItemContentVersion": 1
}
```
