## Account Web - Creator Programs: Creator

URL: https://www.epicgames.com/account/v2/api/creator-programs/creator \
Method: GET \
Auth Required: Yes

---

_Example Response_

```json
{
  "success": true,
  "data": {
    "id": "####",
    "slug": "krowe",
    "programs": [
      {
        "type": "MEDIA",
        "disabledReason": null
      },
      {
        "type": "ISLAND",
        "disabledReason": null
      }
    ],
    "earliestSlugChange": "1970-01-01T00:00:00.000Z",
    "slugChangeInCooldown": false
  }
}
```
