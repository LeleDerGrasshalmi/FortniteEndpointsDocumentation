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
      "linkCode": "7387-6177-4493",
      "linkType": "FG:Creative",
      "sortDate": "2023-08-19T16:44:26.115Z",
      "pagingDate": "2023-08-19T16:44:26.115Z"
    },
    {
      "playerId": "94b1569506b04f9f8557af611e8c5e47",
      "linkCode": "1111-1111-1111",
      "linkType": "Creative:Island",
      "lastVisited": "2023-07-02T15:05:34.452Z",
      "sortDate": "2023-05-30T17:52:16.271Z",
      "pagingDate": "2023-05-30T17:52:16.271Z"
    }
  ],
  "hasMore": false
}
```
