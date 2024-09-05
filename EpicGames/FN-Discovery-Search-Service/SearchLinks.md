## FN - Discovery Search Service - Search Links

URL: https://fn-service-discovery-search-live-public.ogs.live.on.epicgames.com/api/v1/search \
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
      "linkCode": "1334-2993-7207",
      "isFavorite": false,
      "lastVisited": null,
      "globalCCU": 3,
      "score": 9.348631,
      "lockStatus": "UNLOCKED",
      "lockStatusReason": "NONE"
    }
  ]
}
```
