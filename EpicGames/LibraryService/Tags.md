## Library Service - Tags

Localized names of the store tags of one group. Library items list their tags by id (see [Library Items](./V2/LibraryItems.md)).

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/tags \
Method: GET \
Auth Required: Yes (`library:public:tags READ`)

## Query Parameters

`groupName`: `genre`, `feature` or `epicfeature` <br/>
`locale`: Language, e.g. `en`

---

_Example Response (shortened)_

```json
{
  "elements": [
    {
      "id": "1216",
      "name": "Action",
      "groupName": "genre"
    },
    {
      "id": "1117",
      "name": "Adventure",
      "groupName": "genre"
    }
  ],
  "total": 38
}
```

`epicfeature` contains `Achievements` (`19847`) and `Cloud Saves` (`21894`). A user token of the `egs-desktop` client (`c85f4c6238b04d3399bc0080e83b83fc`) has the permission; a `launcherAppClient2` token gets `errors.com.epicgames.common.missing_permission` (403).
