## FN - Discovery Service: Discovery Surface (V2)

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v2/discovery/surface/:surfaceName \
Method: POST \
Auth Required: Yes (`discovery:surface:query READ`)

## Headers

`X-Epic-Access-Token`: The [current discovery access token](/EpicGames/FN-Service/Game/Creative/DiscoveryAccessToken.md)

<br/>

```json
{
  "playerId": "94b1569506b04f9f8557af611e8c5e47",
  "partyMemberIds": ["94b1569506b04f9f8557af611e8c5e47"],
  "accountLevel": 4238,
  "battlepassLevel": 108,
  "locale": "en",
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

`playerId`: Your Account Id <br/>
`partyMemberIds`: Array of the party member account ids (or an empty array) <br/>
`accountLevel`: Your Total alltime level from the athena profile <br/>
`battlepassLevel`: Your current level <br/>
`locale`: Defines in which locale the panel names and data should be <br/>
`matchmakingRegion`: Your matchmaking region (e.g. `EU`) <br/>
`platform`: Your platform <br/>
`isCabined`: If your Account is in Cabined Mode (from [own account info](../../../AccountService/Account/Lookup/AccountId.md)) <br/>
`ratingAuthority`: The Authority used by the client e.g. `USK` <br/>
`rating`: The Rating expected by the client for the given authority, e.g. `USK_AGE_12` for USK 12+ <br/>
`numLocalPlayers`: The count of players in the party

> Technically the request wont fail if you send an empty payload

## Query Parameters

`appId`: `Fortnite` <br/>
`stream`: The Fortnite Branch (URL Encoded), so the branch `++Fortnite+Release-26.30` would need to be encoded like `%2B%2BFortnite%2BRelease-26.30`

---

_Example Response (shortened)_

```json
{
  "testVariantName": "Baseline",
  "testName": "31.30_31.40_EpicPage",
  "testAnalyticsId": "v2|5117|1cf3c6c8329b7f8040f39fec1712d1dd",
  "testVariantAnalyticsId": "v2_v0_c7790",
  "panels": [
    {
      "panelName": "Featured_EpicPage",
      "panelDisplayName": "Featured",
      "panelSubtitle": null,
      "featureTags": [
        "hasViewAll:true",
        "horizontalScroll:false",
        "maxVisibleRows:2",
        "panelType:featured",
        "showIfEmpty:false",
        "squareTiles:false"
      ],
      "firstPage": {
        "results": [
          {
            "lastVisited": "2024-08-31T10:40:42.535Z",
            "linkCode": "playlist_juno",
            "isFavorite": true,
            "globalCCU": 56152,
            "lockStatus": "UNLOCKED",
            "lockStatusReason": "RATING_THRESHOLD",
            "isVisible": true
          }
        ],
        "hasMore": false,
        "panelTargetName": null,
        "pageMarker": null
      },
      "panelType": "CuratedList",
      "playHistoryType": null,
      "panelContexts": {}
    },
    {
      "panelName": "PublishedIslands",
      "panelDisplayName": "More Islands",
      "panelSubtitle": null,
      "featureTags": [
        "hasViewAll:true",
        "horizontalScroll:false",
        "maxVisibleRows:2",
        "panelType:published",
        "showIfEmpty:false",
        "squareTiles:false"
      ],
      "firstPage": {
        "results": [],
        "hasMore": false,
        "panelTargetName": null,
        "pageMarker": null
      },
      "panelType": "PublishedIslands",
      "playHistoryType": null,
      "panelContexts": {}
    }
  ]
}
```
