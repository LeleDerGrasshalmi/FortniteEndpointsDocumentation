## Fortnite - Creative Discovery Panel Page

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v1/discovery/surface/page/:accountId?appId=Fortnite \
Method: POST \
Auth Required: Yes

## Headers

User-Agent: `Fortnite/++Fortnite+Release-{versionNumber}-CL-{versionCL} Windows/10` \
eg. `Fortnite/++Fortnite+Release-18.40-CL-18163738 Windows/10`

## Body

```json
{
  "surfaceName": "CreativeDiscoverySurface_Frontend",
  "panelName": "Competitive",
  "pageIndex": 1,
  "revision": -1,
  "testCohorts": ["c210_baseline"],
  "partyMemberIds": [":accountId"],
  "matchmakingRegion": "EU"
}
```

## Parameter

`surfaceName`: leave as 'CreativeDiscoverySurface_Frontend'
`panelName`: The panel you want to load a different page of
`pageIndex`: The page you want to load from the panel
`revision`: leave -1 for latest
`testCohorts`: grabbed from the main discovery api (<root>.testCohorts)
`partyMemberIds`: array of the party member ids, or an empty array
`matchmakingRegion`: your matchmaking region
