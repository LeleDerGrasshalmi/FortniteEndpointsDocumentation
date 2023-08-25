## Library Service - Get Collections Items

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/collection/account/:accountId \
Method: PUT \
Auth Required: Yes (`library:public:{accountId}:collection UPDATE`)

```json
{
  "name": "Hi GitHub, it's Lele"
}
```

## Path Parameters

`collectionId`: The Collection Id to update (UUIDv4) <br/>
`accountId`: Your Account Id

## Parameters

`name`: The name of the new Collection

---

_Example Response_

```json
{
  "collectionId": "55d39f5c-2253-47da-9224-cf45daec27c2",
  "name": "Hi GitHub, it's Lele",
  "libraryItemContentVersion": 1
}
```
