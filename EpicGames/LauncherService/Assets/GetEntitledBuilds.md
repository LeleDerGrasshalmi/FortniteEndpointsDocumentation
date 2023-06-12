## Launcher Service - Assets: Entitled Builds

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/:platform \
Method: GET \
Auth Required: Yes (`launcher:download:{label} READ`)

## Path Parameters

`platform`: See [Platforms](../README.md#data)

## Query Parameters

`label`: optional, The label, usually `Live`, defaults to `Production` <br/>
`count`: optional, e.g. `1` <br/>
`namespace`: optional, e.g. `fn`

---

_Example Response (shortened)_

```json
[
  {
    "appName": "Fortnite_Studio",
    "labelName": "Live-Windows",
    "buildVersion": "++Fortnite+Release-24.40-CL-25595478-Windows",
    "catalogItemId": "1e8bda5cfbb641b9a9aea8bd62285f73",
    "namespace": "fn",
    "metadata": {
      "installationPoolId": "FortniteInstallationPool"
    },
    "assetId": "Fortnite"
  },
  {
    "appName": "Fortnite",
    "labelName": "Live-Windows",
    "buildVersion": "++Fortnite+Release-24.40-CL-25595478-Windows",
    "catalogItemId": "4fe75bbc5a674f4f9b356b5c90567da5",
    "namespace": "fn",
    "metadata": {
      "installationPoolId": "FortniteInstallationPool"
    },
    "assetId": "Fortnite"
  },
  {
    "appName": "afdb5a85efcc45d8ae8e406e2121d81c",
    "labelName": "Live-Windows",
    "buildVersion": "1.1",
    "catalogItemId": "d75daf91c89b49ecb110b69a7bd68996",
    "namespace": "fn",
    "metadata": {
      "installationPoolId": "FortniteInstallationPool"
    },
    "assetId": "afdb5a85efcc45d8ae8e406e2121d81c"
  },
  {
    "appName": "WorldExplorersLive",
    "labelName": "Live-Windows",
    "buildVersion": "1.88.244-r17036752-Windows",
    "catalogItemId": "a53e821fbdc24181877243a8dbb63463",
    "namespace": "wex",
    "assetId": "WorldExplorersLive"
  }
]
```
