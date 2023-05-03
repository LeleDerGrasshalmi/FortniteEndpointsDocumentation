## Fortnite - Creative Discovery Panel Page

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v1/discovery/surface/page/:accountId \
Method: POST \
Auth Required: Yes (`discovery:{accountId}:surface:query READ`)

## Headers

`User-Agent`:

- Format: `Fortnite/++Fortnite+Release-{major}.{minor}-CL-{changelist} {platform}/{platformVersion}` <br/>
- Example: `Fortnite/++Fortnite+Release-18.40-CL-18163738 Windows/10`

<br/>

```json
{
  "surfaceName": "CreativeDiscoverySurface_Frontend",
  "panelName": "Competitive",
  "pageIndex": 1,
  "revision": -1,
  "testCohorts": [""],
  "partyMemberIds": [""],
  "matchmakingRegion": "",
  "isCabined": true,
  "platform": ""
}
```

## Parameter

`surfaceName`: leave as 'CreativeDiscoverySurface_Frontend' \
`panelName`: The panel you want to load a different page of \
`pageIndex`: The page you want to load from the panel \
`revision`: leave -1 for latest \
`testCohorts`: grabbed from the Main Discovery API (<root>.testCohorts) \
`partyMemberIds`: Array of the party member ids, or an Empty Array \
`matchmakingRegion`: Your matchmaking region (e.g. EU) \
`isCabined`: If your Account is in Cabined Mode (like content/parental controls) \
`platform`: Your platform

## Query Parameter

`appId`: 'Fortnite'
