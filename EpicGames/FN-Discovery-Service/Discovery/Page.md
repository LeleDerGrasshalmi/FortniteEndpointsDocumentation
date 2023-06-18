## FN - Discovery Service: Discovery Surface (Page)

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v1/discovery/surface/page/:accountId \
Method: POST \
Auth Required: Yes (`discovery:{accountId}:surface:query READ`)

## Headers

`User-Agent`: From FN, e.g. `Fortnite/++Fortnite+Release-18.40-CL-18163738 Windows/10`

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
  "platform": "Windows"
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`surfaceName`: Leave as 'CreativeDiscoverySurface_Frontend' <br/>
`panelName`: The panel you want to load a different page of <br/>
`pageIndex`: The page you want to load from the panel <br/>
`revision`: Leave -1 for latest <br/>
`testCohorts`: Grabbed from the [Main Discovery API](./Main.md) (<root>.testCohorts) <br/>
`partyMemberIds`: Array of the party member ids, or an Empty Array <br/>
`matchmakingRegion`: Your matchmaking region (e.g. EU) <br/>
`isCabined`: If your Account is in Cabined Mode (like content/parental controls) <br/>
`platform`: Your platform

## Query Parameters

`appId`: `Fortnite`

---

_Example Response (shortened)_

```json
{
  "results": [
    {
      "lastVisited": null,
      "linkCode": "playlist_nobuildbr_solo",
      "isFavorite": false,
      "globalCCU": 58843
    }
  ],
  "hasMore": false
}
```
