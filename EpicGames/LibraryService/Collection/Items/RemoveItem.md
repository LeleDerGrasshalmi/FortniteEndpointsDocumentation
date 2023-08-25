## Library Service - Remove Item to Collection

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/collection/:collectionId/item/account/:accountId/sandbox/:sandboxId/catalog/:catalogId/artifact/:artifactId \
Method: DELETE \
Auth Required: Yes (`library:public:{accountId}:collection:item DELETE`)

## Path Parameters

`collectionId`: The Collection Id (UUIDv4) <br/>
`accountId`: Your Account Id <br/>
`sandboxId`: The Sandbox Id of the Item (Namespace of the Catalog Item), e.g. `33956bcb55d4452d8c47e16b94e294bd` for Among Us <br/>
`catalogId`: The Catalog Item Id, e.g. `729a86a5146640a2ace9e8c595414c56` for Among Us <br/>
`artifactId`: The Artifact Id of the Item (`appId` of the Catalog Item inside `releaseInfo`), e.g. `963137e4c29d4c79a81323b8fab03a40` for Among Us

---

_Example Response_

```json
{
  "collectionId": "55d39f5c-2253-47da-9224-cf45daec27c2",
  "name": "Hi GitHub, it's Lele",
  "libraryItemContentVersion": 3
}
```
