## Library Service - Items (V2)

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/v2/items \
Method: GET \
Auth Required: Yes

## Query Parameters

`includeMetadata`: (bool), if metadata (for next request) should be inside the response body <br/>
`count`: optional, maximum returned records, capped at `100` (e.g. `500` still returns max 100 Records) <br/>
`includeCategories`: Only include records where the catalog item/offer has the specified category (can be used multiple times), e.g. `games`, `software`, `engines`, `digitalextras`, `mods`, `addons`, `subscription` <br/>
`cursor`: The `nextCursor` from the metadata of the last request, base64 encoded json like `{"offset":100}` (`eyJvZmZzZXQiOjEwMH0=`)

---

_Example Response (shortened)_

A page can contain less records than requested and still have a `nextCursor`, there are no more pages when `nextCursor` is missing. The `stateToken` can be checked with [State Token](../StateToken.md).

```json
{
  "responseMetadata": {
    "nextCursor": "eyJvZmZzZXQiOjEwMH0=",
    "stateToken": "3d9a6f1e-7b2c-4e8a-9f5d-1c2b3a4e5f60"
  },
  "records": [
    {
      "namespace": "5b325322a4c04b9e9e780b9a1e9b2d70",
      "catalogItemId": "9d60f0d4300a407e817ce5548f12f12d",
      "appName": "Grunt",
      "productId": "ca72a212479d4f658b053d06fa37330e",
      "sandboxName": "Aztez",
      "sandboxType": "PUBLIC",
      "recordType": "APPLICATION",
      "acquisitionDate": "2020-02-17T19:37:32.328Z",
      "dependencies": [],
      "tags": [
        {
          "id": "1216",
          "name": "Action",
          "groupName": "genre"
        },
        {
          "id": "1370",
          "name": "Single Player",
          "groupName": "feature"
        }
      ]
    }
  ]
}
```
