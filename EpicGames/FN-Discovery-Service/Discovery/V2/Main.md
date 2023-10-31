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
  "isCabined": false
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
`platform`: Your platform
`isCabined`: If your Account is in Cabined Mode (from [own account info](../../../AccountService/Account/Lookup/AccountId.md))

> Technically the request wont fail if you send an empty payload

## Query Parameters

`appId`: `Fortnite` <br/>
`stream`: The Fortnite Branch (URL Encoded), so the branch `++Fortnite+Release-26.30` would need to be encoded like `%2B%2BFortnite%2BRelease-26.30`

---

_Example Response (shortened)_

```json
{
  "testVariantName": "BrowseVariant1",
  "testName": "BrowseManyVariants_DiffFeatured",
  "testAnalyticsId": "v2|939|9c3e989d15fcfceb4ea90f08af55ad67",
  "testVariantAnalyticsId": "v2_v1_c1396",
  "panels": [
    {
      "panelName": "Featured_B",
      "panelDisplayName": "Featured",
      "featureTags": null,
      "firstPage": {
        "results": [
          {
            "lastVisited": null,
            "linkCode": "reference_panel_new_combat",
            "isFavorite": false,
            "globalCCU": -1
          },
          {
            "lastVisited": null,
            "linkCode": "reference_panel_horror",
            "isFavorite": false,
            "globalCCU": -1
          }
        ],
        "hasMore": false,
        "panelTargetName": null
      },
      "panelType": "CuratedList",
      "playHistoryType": null
    },
    {
      "panelName": "BrowseNewUpdatesThisWeek",
      "panelDisplayName": "New Updates This Week",
      "featureTags": null,
      "firstPage": {
        "results": [
          {
            "lastVisited": null,
            "linkCode": "0482-1284-7823",
            "isFavorite": false,
            "globalCCU": 166
          },
          {
            "lastVisited": null,
            "linkCode": "4196-3017-8839",
            "isFavorite": false,
            "globalCCU": -1
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
