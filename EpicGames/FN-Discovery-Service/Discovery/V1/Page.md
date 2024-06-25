## FN - Discovery Service: Discovery Surface Page (V1)

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v1/discovery/surface/page/:accountId \
Method: POST \
Auth Required: Yes (`discovery:{accountId}:surface:query READ`)

## Headers

`User-Agent`: From FN, e.g. `Fortnite/++Fortnite+Release-18.40-CL-18163738 Windows/10`

<br/>

```json
{
  "surfaceName": "",
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

`surfaceName`: See [Surfaces](../README.md#surfaces) <br/>
`panelName`: The panel you want to load a different page of <br/>
`pageIndex`: The page you want to load from the panel <br/>
`revision`: Leave -1 for latest <br/>
`testCohorts`: Grabbed from the [Main Surface Data](./Main.md) (`testCohorts`) <br/>
`partyMemberIds`: Array of the party member account ids (or an empty array) <br/>
`matchmakingRegion`: Your matchmaking region (e.g. `EU`) <br/>
`isCabined`: If your Account is in Cabined Mode (from [own account info](../../../AccountService/Account/Lookup/AccountId.md)) <br/>
`platform`: Your platform (e.g. `Windows`)

## Query Parameters

`appId`: `Fortnite`

---

_Example Response (shortened)_

```json
{
  "results": [
    {
      "linkCode": "campaign",
      "isFavorite": true,
      "globalCCU": 45383,
      "lockStatus": "UNLOCKED",
      "lockStatusReason": "NONE",
      "isVisible": true
    }
  ],
  "hasMore": false
}
```
