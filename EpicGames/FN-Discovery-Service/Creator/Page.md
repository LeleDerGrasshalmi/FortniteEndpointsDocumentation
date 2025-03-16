## FN - Discovery Service: Creator Islands

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v1/creator/page/:creatorAccountId \
Method: GET \
Auth Required: Yes (`discovery:{accountId}:creator:page READ` - Your Account Id)

## Path Parameters

`creatorAccountId`: Account Id of the Account you want to view the published islands of

## Query Parameters

`playerId`: Your Account Id <br/>
`limit`: Count of Results (Limit is 100) <br/>
`olderThan`: For pagination, when there are more links than the specified page size

---

_Example Response_

```json
{
  "creatorId": "epic",
  "links": [
    {
      "linkCode": "set_habanero_nobuild_blastberry_playlists",
      "lastActivatedDate": "2024-07-26T19:18:11.047Z",
      "isFavorite": false,
      "globalCCU": 55827,
      "lockStatus": "UNLOCKED",
      "lockStatusReason": "RATING_THRESHOLD",
      "isVisible": true
    },
    {
      "linkCode": "campaign",
      "isFavorite": true,
      "globalCCU": 16647,
      "lockStatus": "UNLOCKED",
      "lockStatusReason": "RATING_THRESHOLD",
      "isVisible": true
    }
  ],
  "hasMore": false
}
```
