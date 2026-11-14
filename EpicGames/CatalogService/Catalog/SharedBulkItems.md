## Catalog Service - Shared Bulk Items

Like [Bulk Items](./BulkItems.md), but without a namespace: items from different namespaces can be requested together, and items you do not own are returned too.

URL: https://catalog-public-service-prod06.ol.epicgames.com/catalog/api/shared/bulk/items \
Method: GET \
Auth Required: Yes

## Query Parameters

`id`: Catalog Item Id, repeat for multiple items <br/>
`includeDLCDetails`: `true` / `false` <br/>
`includeMainGameDetails`: `true` / `false` <br/>
`country`: Country code, e.g. `US` <br/>
`locale`: Locale, e.g. `en-US`

---

_Example Response (shortened)_

```json
{
  "4fe75bbc5a674f4f9b356b5c90567da5": {
    "id": "4fe75bbc5a674f4f9b356b5c90567da5",
    "title": "Fortnite",
    "namespace": "fn",
    "status": "ACTIVE",
    "itemType": "DURABLE",
    "entitlementType": "EXECUTABLE",
    "entitlementName": "Fortnite",
    "developer": "Epic Games",
    "eulaIds": ["epicgames_tos"],
    "categories": [{ "path": "games" }, { "path": "applications" }],
    "releaseInfo": [
      {
        "id": "6eec1fba0c494bb8bf157073483ffc4e",
        "appId": "Fortnite",
        "compatibleApps": [],
        "platform": ["Windows", "Mac", "Android"],
        "dateAdded": "2014-09-11T00:00:00.000Z"
      }
    ],
    "dlcItemList": [{ "id": "d75daf91c89b49ecb110b69a7bd68996", "namespace": "fn", "unsearchable": false }],
    "mainGameItemList": []
  },
  "530145df28a24424923f5828cc9031a1": {
    "id": "530145df28a24424923f5828cc9031a1",
    "title": "Rocket League®",
    "namespace": "9773aa1aa54f4f7b80e44bef04986cea"
  }
}
```
