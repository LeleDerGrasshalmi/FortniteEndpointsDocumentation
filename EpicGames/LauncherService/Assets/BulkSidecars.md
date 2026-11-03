## Launcher Service - Assets: Bulk Sidecars

Despite the `PUT` method this is a read, it only returns the sidecars of the requested apps. Apps without a sidecar are left out.

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/bulk/sidecars Method: PUT Auth Required: Yes

```json
[
  {
    "namespace": "37baf50c268d47779020d73143bb02b0",
    "catalogItemId": "fbd21ae74fe24bfa972828c85d43bdd1",
    "appName": "Chicken"
  },
  {
    "namespace": "fn",
    "catalogItemId": "4fe75bbc5a674f4f9b356b5c90567da5",
    "appName": "Fortnite"
  }
]
```

## Parameters

`namespace`: The Catalog Namespace <br/>
`catalogItemId`: The Catalog-Item Id, required and must be unique within the request <br/>
`appName`: The App Name (from Catalog Item)

---

_Example Response_

`config` is a stringified json object, `rvn` the sidecar revision. If none of the requested apps has a sidecar, `data` is empty.

```json
{
  "data": [
    {
      "config": "{  \"deploymentId\" : \"2bcff9c95ae646b78347e46805b79845\"}",
      "rvn": 1,
      "appName": "Chicken",
      "namespace": "37baf50c268d47779020d73143bb02b0"
    }
  ]
}
```

_Example Response (Duplicate catalogItemId)_

```json
{
  "errorCode": "errors.com.epicgames.launcher.bad_argument",
  "errorMessage": "Duplicated catalog items detected: SidecarKey{appName='UE_4.8', namespace='ue', catalogItemId='3ddb1bad6e004b99a7192c1a29f2318a'} | SidecarKey{appName='UE_4.4', namespace='ue', catalogItemId='3ddb1bad6e004b99a7192c1a29f2318a'}",
  "messageVars": [
    "SidecarKey{appName='UE_4.8', namespace='ue', catalogItemId='3ddb1bad6e004b99a7192c1a29f2318a'}",
    "SidecarKey{appName='UE_4.4', namespace='ue', catalogItemId='3ddb1bad6e004b99a7192c1a29f2318a'}"
  ],
  "numericErrorCode": 30016,
  "originatingService": "launcher-service",
  "intent": "prod"
}
```
