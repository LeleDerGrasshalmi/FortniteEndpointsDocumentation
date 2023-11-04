## FN - Discovery Search Service: Search

URL: https://fn-service-discovery-search-live-public.ogs.live.on.epicgames.com/api/v1/search \
Method: POST \
Auth Required: Yes (`discovery:search:{accountId} READ`)

```json
{
  "namespace": "fortnite",
  "context": [],
  "locale": "en-US-POSIX",
  "search": "ssaasaassaa",
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
`orderBy`: What the entries should be ordered by <br/>
`ratingAuthority`: Unknown, iarc? <br/>
`rating`: Unknown <br/>
`page`: Paging

## Query Parameters

`accountId`: Your Account Id

---

_Example Response_

```json
{
  "page": 0,
  "results": [
    {
      "linkCode": "1111-1111-1111",
      "globalCCU": -1
    }
  ]
}
```

> Example Response is not complete, because the service is not enabled yet (as of 04.11.2023)
