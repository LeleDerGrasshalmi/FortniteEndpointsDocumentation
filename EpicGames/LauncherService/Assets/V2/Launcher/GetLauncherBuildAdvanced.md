## Launcher Service - Assets (V2): Launcher Build for Platform (Advanced)

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/v2/platform/:platform/launcher/label/:label \
Method: POST \
Auth Required: Yes (No perm required)

```json
{
  "abis": ["arm64-v8a", "armeabi-v7a", "armeabi"],
  "apiLevel": 30,
  "coreCount": 8,
  "hardwareName": "Qualcomm Technologies, Inc SDMMAGPIE",
  "hasLibHoudini": false,
  "machineId": "REDACTED",
  "manufacturer": "samsung",
  "memoryMiB": 5524,
  "model": "SM-A715F",
  "platform": "Android",
  "preInstallInfo": "ThirdPartyInstall",
  "renderingDevice": "Adreno (TM) 618",
  "renderingDriver": "OpenGL ES 3.2 V@0502.0 (GIT@e1ac91e, I2b3b5fbd00, 1605636002) (Date:11/17/20)",
  "sha1Fingerprint": "",
  "supportsArmNEON": true,
  "supportsFpRenderTargets": true,
  "textureCompressionFormats": ["ASTC", "ATC", "ETC2", "ETC1"],
  "version": "5.2.0"
}
```

## Path Parameters

`platform`: See [Platforms](../../../README.md#data) <br/>
`label`: The label, e.g. `Live-AnarchyAcres` on `Android` or `Live-HighlandWarrior` on `Windows`

## Parameters

`abis`: Array of ABI's, for example see [Android ABI's](https://developer.android.com/ndk/guides/abis) <br/>
`apiLevel`: On Android the [Android API Version](https://developer.android.com/tools/releases/platforms) <br/>
`coreCount`: How many Cores your CPU has <br/>
`hardwareName`: CPU Name <br/>
`hasLibHoudini`: See [What this is](https://commonsware.com/blog/2013/11/21/libhoudini-what-it-means-for-developers.html) <br/>
`machineId`: String <br/>
`manufacturer`: Device Manufacturer, e.g. `samsung` <br/>
`memoryMiB`: Integer <br/>
`model`: Device Model <br/>
`platform`: See [Platforms](../../../README.md#data) <br/>
`preInstallInfo`: Unknown, e.g. `ThirdPartyInstall` <br/>
`renderingDevice`: Graphicscard Name / The name of whatever Device is used for redendering <br/>
`renderingDriver`: Graphicscard / Renderering Device Driver Name and Version <br/>
`sha1Fingerprint`: Empty String when requesting the Launcher build, or the SHA1 Fingerprint of your Devicec <br/>
`supportsArmNEON`: If the CPU sppports [Arm Neon](https://developer.arm.com/Architectures/Neon) <br/>
`supportsFpRenderTargets`: Boolean <br/>
`textureCompressionFormats`: Supported Compression Formats <br/>
`version`: String <br/>

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
