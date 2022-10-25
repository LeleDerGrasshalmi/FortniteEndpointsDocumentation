## Fortnite - Creative Discovery

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
  "revision": -1,
  "partyMemberIds": [":accountId"],
  "matchmakingRegion": "EU"
}
```

## Parameter

`surfaceName`: leave as 'CreativeDiscoverySurface_Frontend' \
`revision`: leave -1 for latest \
`partyMemberIds`: Array of the party member ids, or an Empty Array \
`matchmakingRegion`: Your matchmaking region (e.g. EU)
