## Player Overview Page Service: Get Player Page (Bulk)

URL: https://pops-api-live-public.ogs.live.on.epicgames.com/page/v1 <br/>
Method: POST <br/>
Auth Required: Yes (`pops:playerpage:{accountId} READ`)

```json
{
  "playerIds": ["epic", "37ddc96fe9714096b539967010399670"]
}
```

## Parameters

`playerIds`: Pages Player Account Ids

## Query Parameters

`playerId`: Your Account Id <br/>
`locale`: Your locale, ex. `en`

---

*Example Response*

```json
{
  "results": [
    {
      "playerId": "37ddc96fe9714096b539967010399670",
      "displayName": "pandvil",
      "isFollowed": false,
      "images": {
        "avatar": "https://cdn-0001.qstv.on.epicgames.com/06xTpVCh5zKWvOBU3idIw3/image.jpg",
        "banner": null
      }
    },
    {
      "playerId": "epic",
      "displayName": "Epic Games",
      "isFollowed": false,
      "images": {
        "avatar": "https://cdn2.unrealengine.com/epicgames-cretorprofile-192x192-cd5708661249.jpg",
        "banner": null
      }
    }
  ]
}
```
