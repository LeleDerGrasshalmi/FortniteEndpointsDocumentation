## Player Overview Page Service: Get Player Page

URL: https://pops-api-live-public.ogs.live.on.epicgames.com/page/v1/:pagePlayerId \
Method: GET \
Auth Required: Yes (`pops:playerpage:{accountId} READ`)

## Path Parameters

`pagePlayerId`: Page Player's Account Id

## Query Parameters

`playerId`: Your Account Id

---

_Example Response_

```json
{
  "isFollowed": true,
  "displayName": "Epic Games",
  "surfaceName": "CreativeDiscoverySurface_EpicPage",
  "bio": "Play Fortnite your way. Choose an island and drop in!",
  "followerCount": 2536748,
  "images": {
    "avatar": "https://cdn2.unrealengine.com/epicgames-cretorprofile-192x192-cd5708661249.jpg",
    "banner": "https://cdn2.unrealengine.com/epic-creator-profile-no-logo-2800x960-b1cee1ac257e.jpg"
  },
  "social": {
    "youtube": "fortnite",
    "tikTok": "@fortnite",
    "twitter": "FortniteGame",
    "discord": "fortnite",
    "instagram": "fortnite"
  }
}
```

_Example Response (Has no player page)_: Status 404
