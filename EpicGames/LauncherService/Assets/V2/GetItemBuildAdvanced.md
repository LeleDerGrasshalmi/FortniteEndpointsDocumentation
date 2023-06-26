## Launcher Service - Assets (V2): Get Item Build (Advanced)

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/v2/platform/:platform/namespace/:namespace/catalogItem/:catalogItemId/app/:appName/label/:label \
Method: POST \
Auth Required: Yes (`launcher:download:{label}:{appName} READ`)

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

`platform`: See [Platforms](../../README.md#data) <br/>
`namespace`: The Catalog Namespace, e.g. `fn` for Fortnite <br/>
`catalogItemId`: The Catalog-Item Id, e.g. `4fe75bbc5a674f4f9b356b5c90567da5` for Fortnite <br/>
`appName`: The App Name (from Catalog Item), e.g. `Fortnite` for Fortnite <br/>
`label`: The label, usually `Live`, defaults to `Production`

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
      "appName": "Fortnite",
      "labelName": "Live-Android",
      "buildVersion": "++Fortnite+Release-25.00-CL-25695576-Shipping-Android",
      "hash": "0a6bf0ced25badee2082ed203de8682540547e33",
      "useSignedUrl": false,
      "metadata": {
        "downloadSizeBytes": 137700000,
        "androidPackageName": "com.epicgames.fortnite",
        "androidSigningFingerprintSHA1": "9F:09:41:6D:C4:17:59:9E:63:81:04:22:11:B7:96:40:1F:E2:16:98",
        "androidPackageVersionCode": "25695576",
        "androidSigningFingerprintSHA256": "88:ED:64:07:7B:CA:B1:D2:02:AC:F9:05:F1:60:E4:ED:6C:D5:8E:66:18:2F:A8:13:FC:A4:49:01:0F:2C:C5:05",
        "androidVersionName": "25.00.0-25695576-Android",
        "androidRequiredPermissions": "[\"android.permission.INTERNET\",\"android.permission.ACCESS_NETWORK_STATE\",\"android.permission.WAKE_LOCK\",\"com.android.vending.CHECK_LICENSE\",\"android.permission.ACCESS_WIFI_STATE\",\"android.permission.RECEIVE_BOOT_COMPLETED\",\"android.permission.MODIFY_AUDIO_SETTINGS\",\"android.permission.VIBRATE\",\"com.android.vending.BILLING\",\"android.permission.BLUETOOTH\",\"android.permission.RECORD_AUDIO\",\"com.samsung.android.iap.permission.BILLING\",\"android.permission.GET_ACCOUNTS\",\"android.permission.FOREGROUND_SERVICE\",\"com.google.android.c2dm.permission.RECEIVE\",\"com.epicgames.fortnite.permission.C2D_MESSAGE\"]"
      },
      "manifests": [
        {
          "uri": "https://download2.epicgames.com/Builds/Fortnite/CloudDir/fjxwON6Cfk_5yELu9EqXzS0RjQmyrQ.manifest",
          "queryParams": [
            {
              "name": "Policy",
              "value": "eyJTdGF0ZW1lbnQiOiBbeyJSZXNvdXJjZSI6IiovQnVpbGRzL0ZvcnRuaXRlL0Nsb3VkRGlyL2ZqeHdPTjZDZmtfNXlFTHU5RXFYelMwUmpRbXlyUS5tYW5pZmVzdCIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTY4NjUwNTAzNn0sIklwQWRkcmVzcyI6eyJBV1M6U291cmNlSXAiOiIwLjAuMC4wLzAifX19XX0_"
            },
            {
              "name": "Signature",
              "value": "t0G34ZpvZ83K1~28mZS2JEtawCVeAOrDgS36V5YQS9Eb190xeIfYv18Xxp6YUZeQCdPcsgkWV64Ge3Nql-Bs0vt3Lqk1Er7vdNMOCdC9yyf1e9iAUiI85SKENCYbI4flCqoPYi9~q2v16~2sX0YqWiqPpUDj83ZNz5g1jZy7PVeUOf~XZnQ4ussUN-QQ2hnR7CCAJs72iOkkll8a43Gv-L6WDhcBQhSn6iyN1meHYgv8vjIbPLblOaMO5xgectG6e5AjsEzKnVh-kbD6KD-~ZZVB9FTXBHX0T9fv7QJXHDsGI63P-j0CuhO-8JTgN1gres25QqQMHzgZuSpMDM12NQ__"
            },
            {
              "name": "Key-Pair-Id",
              "value": "APKAJP7WU44FM4EHJYFQ"
            }
          ]
        }
      ]
    }
  ]
}
```
