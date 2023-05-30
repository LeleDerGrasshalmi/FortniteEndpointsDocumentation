## FN - Discovery Service: Recently-Played Links

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v1/links/history/:accountId \
Method: GET \
Auth Required: Yes (`discovery:{accountId}:links:history READ`)

## Path Parameters

`accountId`: Your Account Id

## Query Parameters

`limit`: optional, e.g. `50`

---

_Example Response_

```json
{
  "results": [
    {
      "playerId": "94b1569506b04f9f8557af611e8c5e47",
      "linkCode": "6276-3568-1807",
      "linkType": "valkyrie:application",
      "lastVisited": "2023-05-30T17:41:17.652Z",
      "isFavorite": true,
      "pagingDate": "2023-05-30T17:41:17.652Z"
    }
  ],
  "hasMore": false
}
```
