## FN - Discovery Search Service - Search Creators

URL: https://fn-service-discovery-search-live-public.ogs.live.on.epicgames.com/api/v1/creators/search \
Method: POST \
Auth Required: Yes (`discovery:search:{accountId} READ`)

```json
{
  "term": "epic"
}
```

## Parameters

`term`: Search Query Input

---

_Example Response (Not working yet)_

```json
{
  "timestamp": 1725056523599,
  "path": "/api/v1/creators/search",
  "status": 500,
  "error": "Internal Server Error",
  "requestId": "fdf04b93-1072598"
}
```
