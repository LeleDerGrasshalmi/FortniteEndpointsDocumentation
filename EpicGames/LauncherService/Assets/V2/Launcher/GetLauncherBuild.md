## Launcher Service - Assets (V2): Launcher Build for Platform

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/v2/platform/:platform/launcher \
Method: GET \
Auth Required: Yes (No perm required)

## Path Parameters

`platform`: See [Platforms](../../../README.md#data)

## Query Parameters

`label`: required, The label, e.g. `Live-AnarchyAcres` on `Android` or `Live-HighlandWarrior` on `Windows` <br/>
`clientVersion`: optional, the Launcher Version, e.g. `15.4.0-25591319+++Portal+Release-Live-Windows` (Needs to get URL Encoded!) <br/>
`machineId`: optional, your hwid, e.g. `BD89F33D-3365-45D1-BA2B-EB4D6B397AE8`

---

_Example Response (shortened)_

```json
{
  "elements": [
    {
      "appName": "EpicGamesLauncher",
      "labelName": "Live-AnarchyAcres-Android",
      "buildVersion": "3.0.1-c6f7580.b41+Releaselive-defaultInstallerRelease-Android",
      "hash": "3ba6d3637498b3a53026fbf52eccf8dc2bc9ecae",
      "useSignedUrl": false,
      "metadata": {
        "buildTime": "2019-04-03T17:22:54Z",
        "androidPackageName": "com.epicgames.portal",
        "androidSigningFingerprintSHA1": "70:75:66:F8:B0:9B:4C:8B:FD:77:2E:1B:53:6D:58:1F:19:BC:30:12",
        "androidPackageVersionCode": "12",
        "label": "StandardInstallReleaselive",
        "androidSigningFingerprintSHA256": "67:69:9A:6B:3D:31:5D:EE:51:53:6A:67:B4:F1:C6:E7:E2:17:5F:98:4B:09:6B:C2:97:6E:51:2D:22:94:08:71",
        "epicBuildVersion": "3.0.1-c6f7580.b41+Releaselive-defaultInstallerRelease-Android"
      },
      "manifests": [
        {
          "uri": "https://fastly-download.epicgames.com/Builds/UnrealEngineLauncher/CloudDir/RcsVeYxFtLoMSFq6N0mchaeri-PLxA.manifest",
          "queryParams": [
            {
              "name": "f_token",
              "value": "1685648904_fc1106f0017084ff25385658f8a5ac618dca4b97"
            }
          ]
        }
      ]
    }
  ]
}
```
