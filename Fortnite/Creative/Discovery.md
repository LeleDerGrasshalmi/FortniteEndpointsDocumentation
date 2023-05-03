## Fortnite - Creative Discovery

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v1/discovery/surface/:accountId \
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
  "revision": -1,
  "partyMemberIds": [":accountId"],
  "matchmakingRegion": "",
  "isCabined": true,
  "platform": ""
}
```

## Parameter

`surfaceName`: leave as 'CreativeDiscoverySurface_Frontend' \
`revision`: leave -1 for latest \
`partyMemberIds`: Array of the party member ids, or an Empty Array \
`matchmakingRegion`: Your matchmaking region (e.g. EU) \
`isCabined`: If your Account is in Cabined Mode (like content/parental controls) \
`platform`: Your platform

## Query Parameter

`appId`: 'Fortnite'
