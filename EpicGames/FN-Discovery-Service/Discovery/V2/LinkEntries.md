## FN - Discovery Service: Discovery Link Entries

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v2/discovery/link-entries \
Method: POST \
Auth Required: Yes (`discovery:surface:query READ`)

```json
{
  "linkCodes": ["playlist_trios"]
}
```

## Parameters

`linkCodes`: Link codes to query the discovery entry from

---

_Example Response_

```json
{
  "playlist_trios": {
    "lastVisited": null,
    "linkCode": "playlist_trios",
    "isFavorite": false,
    "globalCCU": 8720,
    "lockStatus": "UNLOCKED",
    "lockStatusReason": "RATING_THRESHOLD",
    "isVisible": true,
    "favoriteStatus": "NONE"
  }
}
```
