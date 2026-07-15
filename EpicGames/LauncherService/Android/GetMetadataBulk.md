## Launcher Service - Android: Asset Metadata (Bulk)

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/android/v1/metadata/bulk \
Method: POST \
Auth Required: Yes (`launcher:download:android:metadata:bulk READ`)

```json
{
    "androidMetadataKeys": [{
        "namespace": "fn",
        "catalogItemId": "4fe75bbc5a674f4f9b356b5c90567da5",
        "label": "Live"
    }],
    "attributes": {
        "abis": ["arm64-v8a"],
        "apiLevel": 35,
        "coreCount": 8,
        "hardwareName": "generic",
        "manufacturer": "Google",
        "memoryMiB": 8192,
        "model": "Pixel 8",
        "platform": "Android",
        "renderingDevice": "Adreno (TM) 750",
        "renderingDriver": "",
        "textureCompressionFormats": ["ASTC"],
        "version": "15",
        "versionCode": 35,
        "launcher": ""
    }
}
```

---

_Example Response_

```json
{
    "results": [
        {
            "catalogItemId": "4fe75bbc5a674f4f9b356b5c90567da5",
            "namespace": "fn",
            "label": "Live",
            "metadata": {
                "buildVersion": "++Fortnite+Release-41.10-CL-55227503-Shipping-Android",
                "androidPackageName": "com.epicgames.fortnite",
                "androidPackageVersionCode": "55227503",
                "androidVersionName": "41.10.0-55227503-Android",
                "minAndroidSdk": 26,
                "androidRequiredPermissions": "[\"android.permission.INTERNET\",\"android.permission.ACCESS_NETWORK_STATE\",\"com.android.vending.CHECK_LICENSE\",\"android.permission.ACCESS_WIFI_STATE\",\"android.permission.RECEIVE_BOOT_COMPLETED\",\"android.permission.WAKE_LOCK\",\"android.permission.MODIFY_AUDIO_SETTINGS\",\"android.permission.VIBRATE\",\"com.android.vending.BILLING\",\"android.permission.FOREGROUND_SERVICE\",\"android.permission.FOREGROUND_SERVICE_DATA_SYNC\",\"android.permission.POST_NOTIFICATIONS\",\"android.permission.RECORD_AUDIO\",\"com.google.android.c2dm.permission.RECEIVE\",\"com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE\",\"com.epicgames.fortnite.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION\",\"com.samsung.android.iap.permission.BILLING\",\"android.permission.GET_ACCOUNTS\",\"android.permission.BIND_JOB_SERVICE\",\"android.permission.DUMP\",\"com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION\",\"com.google.android.c2dm.permission.SEND\"]",
                "androidSigningFingerprintSHA256": "88:ED:64:07:7B:CA:B1:D2:02:AC:F9:05:F1:60:E4:ED:6C:D5:8E:66:18:2F:A8:13:FC:A4:49:01:0F:2C:C5:05",
                "downloadSizeBytes": 248429062
            }
        }
    ]
}
```
