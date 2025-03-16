## Player Overview Page Service: Get Player Page (Bulk)

URL: https://pops-api-live-public.ogs.live.on.epicgames.com/page/v1 \
Method: POST \
Auth Required: Yes (`pops:playerpage:{accountId} READ`)

```json
{
  "playerIds": ["epic", "37ddc96fe9714096b539967010399670"]
}
```

## Query Parameters

`playerId`: Your Account Id <br/>
`locale`: Your locale, ex. `en`

## Parameters

`playerIds`: Pages Player Account Ids

---

_Example Response_

```json
{
  "results": [
    {
      "playerId": "37ddc96fe9714096b539967010399670",
      "displayName": "pandvil",
      "isFollowed": false,
      "images": {
        "avatar": "https://cdn-0001.qstv.on.epicgames.com/05vZ2nB1k38ZkStczM7WG1/image.jpg",
        "banner": null
      }
    },
    {
      "playerId": "epic",
      "displayName": "Epic Games",
      "isFollowed": true,
      "images": {
        "avatar": "https://cdn2.unrealengine.com/epicgames-cretorprofile-192x192-cd5708661249.jpg",
        "banner": null
      }
    }
  ]
}
```
