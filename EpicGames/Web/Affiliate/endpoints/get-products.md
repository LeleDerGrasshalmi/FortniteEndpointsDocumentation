# Get Earned Products

URL: https://sac.epicgames.com/api/get-products \
Method: GET \
Auth Required: Yes

## Query Parameters

`keywords`: If you are searching for products by their Name <br/>
`locale`: Product Data Language <br/>
`page`: Page Index (paging) <br/>
`start`: Offset (paging) <br/>
`count`: Count of products to return <br/>
`sortBy`: Property the products should be sorted by, e.g `relevancy` <br/>
`sortDir`: Sort Direction (ASC, DESC)

---

_Example Response (shortened)_

```json
{
  "data": {
    "elements": {
      "ef7baa6ce017413ab33e7f7e3f466a96": {
        "namespace": "ef7baa6ce017413ab33e7f7e3f466a96",
        "icon": "https://cdn1.epicgames.com/offer/ef7baa6ce017413ab33e7f7e3f466a96/EGS_Homeworld3_BlackbirdInteractive_S2_1200x1600-2080e2e3662c285b1c9efcb13f3a8d07",
        "title": "Homeworld 3",
        "urlSlug": "homeworld-3",
        "shareRate": 5,
        "pageSlug": "homeworld-3"
      },
      "89018fd416314b829bbf175c0b4aa440": {
        "namespace": "89018fd416314b829bbf175c0b4aa440",
        "icon": "https://cdn1.epicgames.com/spt-assets/947537fa3c924882aebd28869cc125c7/download-superior-offer-1k4rf.jpg",
        "title": "Superior",
        "urlSlug": "665524e24eaa403f822a492ee79c9c4c",
        "shareRate": 5,
        "pageSlug": "superior-0bd6d0"
      }
    },
    "paging": {
      "count": 18,
      "start": 0,
      "total": 2844
    }
  },
  "success": true
}
```
