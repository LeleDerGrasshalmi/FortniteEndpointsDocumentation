## FN - Discovery Search Service - Search Creators

URL: https://fn-service-discovery-search-live-public.ogs.live.on.epicgames.com/api/v1/creators/search \
Method: POST \
Auth Required: Yes (`discovery:search:{accountId} READ`)

```json
{
  "creatorTerm": "epic"
}
```

## Parameters

`creatorTerm`: Creator Search Input

## Query Parameters

`accountId`: Your Account Id

---

_Example Response (shortened)_

```json
{
  "results": [
    {
      "accountId": "epic",
      "score": 4.3400574
    },
    {
      "accountId": "1bd256a05c1842cbbcb1e4133bd47fec",
      "score": 3.7241647
    }
  ]
}
```
