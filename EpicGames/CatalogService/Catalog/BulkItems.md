## Catalog Service - Catalog: Bulk Items

URL: https://catalog-public-service-prod06.ol.epicgames.com/catalog/api/shared/namespace/:namespace/bulk/items \
Method: GET \
Auth Required: Yes

## Path Parameters

`namespace`: The Catalog Namespace, e.g. `fn` for Fortnite

## Query Parameters

`id`: The Catalog-Item Id (can be used multiple times) <br/>
`includeDLCDetails`: (bool), e.g. `true` <br/>
`includeMainGameDetails`: (bool), e.g. `true` <br/>
`country`: e.g. `US` <br/>
`locale`: e.g. `en`

---

_Example Response (shortened)_

```json
{
  "9d60f0d4300a407e817ce5548f12f12d": {
    "id": "9d60f0d4300a407e817ce5548f12f12d",
    "title": "Aztez",
    "description": "Aztez",
    "keyImages": [
      {
        "type": "DieselGameBoxTall",
        "url": "https://cdn1.epicgames.com/5b325322a4c04b9e9e780b9a1e9b2d70/item/EGS_TeamColorblind_Aztez_S2-860x1148-0d2b32f59c7ce18bdb7f2c538c4cb3fa.jpg",
        "md5": "0d2b32f59c7ce18bdb7f2c538c4cb3fa",
        "width": 860,
        "height": 1148,
        "size": 192699,
        "uploadedDate": "2020-02-05T17:35:34.847Z"
      }
    ],
    "categories": [
      {
        "path": "public"
      },
      {
        "path": "games"
      },
      {
        "path": "applications"
      }
    ],
    "namespace": "5b325322a4c04b9e9e780b9a1e9b2d70",
    "status": "ACTIVE",
    "creationDate": "2019-12-05T20:51:43.793Z",
    "lastModifiedDate": "2020-02-06T15:11:50.571Z",
    "customAttributes": {
      "CanRunOffline": {
        "type": "STRING",
        "value": "true"
      },
      "PresenceId": {
        "type": "STRING",
        "value": "5b325322a4c04b9e9e780b9a1e9b2d70"
      },
      "FolderName": {
        "type": "STRING",
        "value": "Aztez"
      }
    },
    "entitlementName": "9d60f0d4300a407e817ce5548f12f12d",
    "entitlementType": "EXECUTABLE",
    "itemType": "DURABLE",
    "releaseInfo": [
      {
        "id": "f729c3179f6743c4b1924c46bad6e050",
        "appId": "Grunt",
        "platform": ["Windows", "Mac"],
        "dateAdded": "2020-02-05T17:36:36.008Z"
      }
    ],
    "developer": "Team Colorblind",
    "developerId": "o-ndzqj36dmhqmfklcq44yywpgfnbmbd",
    "eulaIds": ["egstore"],
    "endOfSupport": false,
    "mainGameItemList": [],
    "ageGatings": {},
    "selfRefundable": true,
    "unsearchable": false
  }
}
```
