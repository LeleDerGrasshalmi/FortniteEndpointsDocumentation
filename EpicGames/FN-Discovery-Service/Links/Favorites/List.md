## FN - Discovery Service: Favorite Links

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v1/links/favorites/:accountId \
Method: GET \
Auth Required: Yes (`discovery:{accountId}:links:favorite READ`)

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
      "linkCode": "5002-6999-0901",
      "linkType": "Reference",
      "sortDate": "2023-04-15T16:56:03.840Z",
      "pagingDate": "2023-04-15T16:56:03.840Z"
    }
  ],
  "hasMore": false
}
```
