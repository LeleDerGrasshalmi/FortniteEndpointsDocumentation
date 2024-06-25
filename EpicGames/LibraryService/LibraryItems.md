## Library Service - Items

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/items \
Method: GET \
Auth Required: Yes (`library:public:items READ`)

## Query Parameters

`includeMetadata`: (bool), if metadata (for next request) should be inside the response body <br/>
`cursor`: From the metadata from last request, or build your own: base64 encoded json like `{"offset":10}` (Will skip the first 10 Records) <br/>
`excludeNs`: Allow to optionally exclude Records from a certain Namespace (can be used multiple times) <br/>
`includeNs`: Allow to optionally include Records from a certain Namespace (can be used multiple times) <br/>
`limit`: Set the Limit of maximum returned records <br/>
`platform`: Only List Records available on the requested platform, e.g. `Windows`, `Android` etc. (Same as Launcher Service) <br/>
`includeCategories`: Only include records where the catalog item/offer has the specified category

---

_Example Response (shortened)_

`responseMetadata` is only included in the body if `includeMetadata` is true, otherwhise it will be returned in the `X-Epic-Metadata` Header.

```json
{
  "responseMetadata": {
    "nextCursor": "eyJvZmZzZXQiOjEwMH0=",
    "stateToken": "aa000214-01b3-460f-b971-a684b6588291"
  },
  "records": [
    {
      "namespace": "fn",
      "catalogItemId": "c6cb1a1d11f54fab8e17301f66bc27a4",
      "productId": "prod-fn",
      "sandboxName": "Fortnite",
      "sandboxType": "PUBLIC",
      "recordType": "SUBSCRIPTION",
      "acquisitionDate": "2020-12-03T17:30:44.370Z",
      "dependencies": []
    },
    {
      "namespace": "fn",
      "catalogItemId": "4fe75bbc5a674f4f9b356b5c90567da5",
      "appName": "Fortnite",
      "productId": "prod-fn",
      "sandboxName": "Fortnite",
      "sandboxType": "PUBLIC",
      "recordType": "APPLICATION",
      "acquisitionDate": "2018-08-21T17:09:17.522Z",
      "dependencies": []
    },
    {
      "namespace": "879b0d8776ab46a59a129983ba78f0ce",
      "catalogItemId": "7d690c122fde4c60bed85405f343ad10",
      "appName": "41869934302e4b8cafac2d3c0e7c293d",
      "productId": "99dc46c68ea14324964a856d18dcac5b",
      "sandboxName": "Genshin Impact",
      "sandboxType": "PUBLIC",
      "recordType": "APPLICATION",
      "acquisitionDate": "2021-06-10T14:26:48.383Z",
      "dependencies": []
    }
  ]
}
```
