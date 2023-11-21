## FN - Discovery Service: Discovery Surface (V2)

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v2/discovery/surface/:surfaceName \
Method: POST \
Auth Required: Yes (`discovery:surface:query READ`)

## Headers

`X-Epic-Access-Token`: The [current discovery access token](/Fortnite/Creative/DiscoveryAccessToken.md)

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
  "rating": "USK_AGE_12"
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
`rating`: The Rating expected by the client for the given authority, e.g. `USK_AGE_12` for USK 12+

> Technically the request wont fail if you send an empty payload

## Query Parameters

`appId`: `Fortnite` <br/>
`stream`: The Fortnite Branch (URL Encoded), so the branch `++Fortnite+Release-26.30` would need to be encoded like `%2B%2BFortnite%2BRelease-26.30`

---

_Example Response (shortened)_

```json
{
  "testVariantName": "V1_EU_1_4",
  "testName": "27.00_11/03/2023_HomebarRPTest",
  "testAnalyticsId": "v2|1011|6e5dfa45cf32e36e3e75c7ac47514fc3",
  "testVariantAnalyticsId": "v2_v22_c1665",
  "panels": [
    {
      "panelName": "Homebar2",
      "panelDisplayName": "Homebar",
      "featureTags": ["col:5", "homebar"],
      "firstPage": {
        "results": [
          {
            "lastVisited": null,
            "linkCode": "reference_joinableparties_2",
            "isFavorite": false,
            "globalCCU": -1,
            "lockStatus": "UNLOCKED",
            "lockStatusReason": "NONE",
            "isVisible": true
          },
          {
            "lastVisited": null,
            "linkCode": "reference_current_island",
            "isFavorite": false,
            "globalCCU": -1,
            "lockStatus": "UNLOCKED",
            "lockStatusReason": "NONE",
            "isVisible": true
          }
        ],
        "hasMore": false,
        "panelTargetName": null
      },
      "panelType": "CuratedList",
      "playHistoryType": null
    },
    {
      "panelName": "ByEpicNoBigBattle6ColRanked",
      "panelDisplayName": "By Epic",
      "featureTags": ["col:5"],
      "firstPage": {
        "results": [
          {
            "lastVisited": "2023-09-24T13:23:39.954Z",
            "linkCode": "playlist_playgroundv2",
            "isFavorite": true,
            "globalCCU": 46479,
            "lockStatus": "UNLOCKED",
            "lockStatusReason": "NONE",
            "isVisible": true
          }
        ],
        "hasMore": false,
        "panelTargetName": null
      },
      "panelType": "AnalyticsList",
      "playHistoryType": null
    }
  ]
}
```
