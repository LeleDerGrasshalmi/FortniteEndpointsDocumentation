## FN - Discovery Service: Discovery Surface Page (V2)

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v2/discovery/surface/:surfaceName/page \
Method: POST \
Auth Required: Yes (`discovery:surface:query READ`)

## Headers

`X-Epic-Access-Token`: The [current discovery access token](/EpicGames/FN-Service/Game/Creative/DiscoveryAccessToken.md)

<br/>

```json
{
  "testVariantName": "BrowseVariant3",
  "panelName": "BrowseNewUpdatesThisWeek",
  "pageIndex": 0,
  "playerId": "94b1569506b04f9f8557af611e8c5e47",
  "partyMemberIds": ["94b1569506b04f9f8557af611e8c5e47"],
  "matchmakingRegion": "EU",
  "platform": "Windows",
  "isCabined": false,
  "ratingAuthority": "USK",
  "rating": "USK_AGE_12",
  "numLocalPlayers": 1
}
```

## Path Parameters

`surfaceName`: See [Surfaces](../README.md#surfaces)

## Parameters

`testVariantName`: From the [Main Discovery Response](./Main.md) <br/>
`panelName`: The panel you want to load a different page of <br/>
`pageIndex`: The page you want to load from the panel <br/>
`partyMemberIds`: Array of the party member account ids (or an empty array) <br/>
`matchmakingRegion`: Your matchmaking region (e.g. `EU`) <br/>
`platform`: Your platform (e.g. `Windows`) <br/>
`isCabined`: If your Account is in Cabined Mode (from [own account info](../../../AccountService/Account/Lookup/AccountId.md)) <br/>
`ratingAuthority`: The Authority used by the client e.g. `USK` <br/>
`rating`: The Rating expected by the client for the given authority, e.g. `USK_AGE_12` for USK 12+ <br/>
`numLocalPlayers`: The count of players in the party

> Technically the request wont fail if only `testVariantName`, `panelName` and `pageIndex` are provided

## Query Parameters

`appId`: `Fortnite` <br/>
`stream`: The Fortnite Branch (URL Encoded), so the branch `++Fortnite+Release-26.30` would need to be encoded like `%2B%2BFortnite%2BRelease-26.30`

---

_Example Response (shortened)_

```json
{
  "results": [
    {
      "lastVisited": null,
      "linkCode": "set_habanero_blastberry_playlists",
      "isFavorite": false,
      "globalCCU": 370554,
      "lockStatus": "UNLOCKED",
      "lockStatusReason": "RATING_THRESHOLD",
      "isVisible": true
    }
  ],
  "hasMore": false,
  "panelTargetName": null,
  "pageMarker": null
}
```
