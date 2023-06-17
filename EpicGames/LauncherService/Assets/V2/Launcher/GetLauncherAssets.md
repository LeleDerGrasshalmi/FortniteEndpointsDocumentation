## Launcher Service - Assets (V2): Launcher Assets for Platform (without Downloads)

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/v2/platform/:platform/launcher/version \
Method: GET \
Auth Required: Yes (`buildinfo:buildmanifest:app:EpicGamesLauncher:build:{version}:status READ` if using `clientVersion`, else None)

## Path Parameters

`platform`: See [Platforms](../../../README.md#data)

## Query Parameters

`label`: required, The label, e.g. `Live-AnarchyAcres` on `Android` or `Live-HighlandWarrior` on `Windows` <br/>
`clientVersion`: optional, the Launcher Version, e.g. `15.4.0-25591319+++Portal+Release-Live-Windows` (Needs to get URL Encoded!)

---

_Example Response (With clientVersion)_

```json
{
  "elements": [
    {
      "appName": "EpicGamesLauncher",
      "labelName": "Live-HighlandWarrior-Windows",
      "buildVersion": "15.6.0-25959195+++Portal+Release-Live-Windows",
      "hash": "647c1e230545f32fa3913f8edc106675fc72bc21",
      "useSignedUrl": false
    },
    {
      "appName": "EpicGamesLauncherContent",
      "labelName": "Live-HighlandWarrior-Windows",
      "buildVersion": "++Portal+Main+prod-CL-26023651-Windows",
      "hash": "069e40ab0298878cb8ed1e0dbeb75da8ae8798ab",
      "useSignedUrl": false
    }
  ],
  "buildStatuses": [
    {
      "app": "EpicGamesLauncher",
      "status": "NOT_DEPRECATED"
    }
  ]
}
```

_Example Response (without clientVersion)_

```json
{
  "elements": [
    {
      "appName": "EpicGamesLauncher",
      "labelName": "Live-HighlandWarrior-Windows",
      "buildVersion": "15.6.0-25959195+++Portal+Release-Live-Windows",
      "hash": "647c1e230545f32fa3913f8edc106675fc72bc21",
      "useSignedUrl": false
    },
    {
      "appName": "EpicGamesLauncherContent",
      "labelName": "Live-HighlandWarrior-Windows",
      "buildVersion": "++Portal+Main+prod-CL-26023651-Windows",
      "hash": "069e40ab0298878cb8ed1e0dbeb75da8ae8798ab",
      "useSignedUrl": false
    }
  ]
}
```
