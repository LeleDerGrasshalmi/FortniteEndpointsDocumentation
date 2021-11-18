## Fortnite - Creative Discovery

URL: https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/game/v2/creative/discovery/surface/:accountId \
Method: POST \
Auth Required: Yes

## Headers
`User-Agent: Fortnite/++Fortnite+Release-{versionNumber}-CL-{versionCL} Windows/10` \
eg. Fortnite/++Fortnite+Release-18.40-CL-18163738 Windows/10

## Body
```json
{
   "surfaceName": "CreativeDiscoverySurface_Frontend",
   "revision": 1,
   "partyMemberIds": [":accountId"]
}
```
NOTE: partyMemberIds can be an be an empty array, but the parameter need to exist in the body
