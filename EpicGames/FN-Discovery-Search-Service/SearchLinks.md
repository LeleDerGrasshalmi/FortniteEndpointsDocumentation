## FN - Discovery Search Service - Search Links

URL: https://fngw-svc-gc-livefn.ol.epicgames.com/api/island-search/v1/search \
Method: POST \
Auth Required: Yes (`discovery:search:{accountId} READ`)

```json
{
  "namespace": "fortnite",
  "context": [],
  "locale": "en-US-POSIX",
  "search": "test",
  "orderBy": "globalCCU",
  "ratingAuthority": "",
  "rating": "",
  "page": 0
}
```

## Parameters

`namespace`: `fortnite` <br/>
`context`: Unknown Array <br/>
`locale`: Language of your input <br/>
`search`: Search Query Input <br/>
`orderBy`: What key the entries should be ordered by <br/>
`ratingAuthority`: The Authority used by the client e.g. `USK` <br/>
`rating`: The Rating expected by the client for the given authority, e.g. `USK_AGE_12` for USK 12+
`page`: Paging

## Query Parameters

`accountId`: Your Account Id

---

_Example Response_

```json
{
  "results": [
    {
      "linkCode": "1269-6181-1603",
      "isFavorite": false,
      "lastVisited": null,
      "globalCCU": 1,
      "score": 2.3827636,
      "lockStatus": "UNLOCKED",
      "lockStatusReason": "RATING_THRESHOLD",
      "isVisible": true
    },
    {
      "linkCode": "6608-3568-6843",
      "isFavorite": true,
      "lastVisited": 1700589249.54,
      "globalCCU": -1,
      "score": 1.5033565,
      "lockStatus": "LOCKED",
      "lockStatusReason": "RATING_THRESHOLD",
      "isVisible": true
    }
  ]
}
```
