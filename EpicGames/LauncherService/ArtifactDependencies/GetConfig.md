## Launcher Service - Artifact Dependencies: Config

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/artifactDependencies/v1/config/:namespace/:catalogItemId/:appName/:buildVersion \
Method: GET \
Auth Required: Yes

## Path Parameters

`namespace`: The Catalog Namespace, e.g. `fn` for Fortnite <br/>
`catalogItemId`: The Catalog-Item Id, e.g. `4fe75bbc5a674f4f9b356b5c90567da5` for Fortnite <br/>
`appName`: The App Name (from Catalog Item), e.g. `Fortnite` for Fortnite <br/>
`buildVersion`: The `buildVersion` from [Get Item Build](../Assets/V2/GetItemBuild.md), e.g. `++Fortnite+Release-42.30-CL-58813929-Windows`

---

_Example Response (shortened)_

Only builds with `metadata.hasDependencyConfig` set to `true` in [Get Item Build](../Assets/V2/GetItemBuild.md) have a config.

```json
{
  "namespace": "fn",
  "baseCatalogItemId": "4fe75bbc5a674f4f9b356b5c90567da5",
  "baseArtifactId": "Fortnite",
  "buildVersion": "++Fortnite+Release-42.30-CL-58813929-Windows",
  "created": "2026-10-06T12:04:14.736Z",
  "rvn": 1,
  "aliases": {
    "Fortnite": "Fortnite",
    "FortniteStWContent": "aa31f9e94e844b299ca757d1d0b97a09",
    "FortniteJunoContent": "94bc5ec13f8f438c97fdbef3e9019e27"
  },
  "entries": {
    "Fortnite": {
      "namespace": "fn",
      "catalogItemId": "4fe75bbc5a674f4f9b356b5c90567da5",
      "dependencies": []
    },
    "aa31f9e94e844b299ca757d1d0b97a09": {
      "namespace": "fn",
      "catalogItemId": "0b41f0192f7f4f2691684581aedc0778",
      "dependencies": ["Fortnite"]
    },
    "94bc5ec13f8f438c97fdbef3e9019e27": {
      "namespace": "fn",
      "catalogItemId": "b619cf61a4144d67bd753dc990637e7c",
      "dependencies": ["Fortnite"]
    }
  }
}
```

_Example Response (404, build without a config)_

```json
{
  "errorCode": "errors.com.epicgames.launcher.artifact_dependency_config_not_found",
  "errorMessage": "No artifact dependency configuration found for namespace=daisy, baseArtifactId=Daisy, buildVersion=1.0.3",
  "messageVars": ["daisy", "Daisy", "1.0.3"],
  "numericErrorCode": 30033,
  "originatingService": "launcher-service",
  "intent": "prod"
}
```
