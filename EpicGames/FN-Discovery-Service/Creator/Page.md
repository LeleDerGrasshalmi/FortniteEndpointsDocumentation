## FN - Discovery Service: Creator Islands

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v1/creator/page/:creatorAccountId \
Method: GET \
Auth Required: Yes (`discovery:{accountId}:creator:page READ` - Your Account Id)

## Path Parameters

`creatorAccountId`: Account Id of the Account you want to view the published islands of

## Query Parameters

`playerId`: Your Account Id <br/>
`limit`: Count of Results (Limit is 100)

---

_Example Response_

```json
{
  "creatorId": "4c2342479c23474daf0c38f64c7d7871",
  "links": [
    {
      "linkCode": "6843-3677-1390",
      "lastActivatedDate": "2023-05-13T23:38:32.569Z",
      "isFavorite": false,
      "globalCCU": 218
    }
  ],
  "hasMore": false
}
```
