## Wex Service - Manifests: ChunkV3

URL: https://wex-public-service-live-prod.ol.epicgames.com/wex/api/game/v2/manifests/:manifest \
Method: GET \
Auth Required: No

## Path Parameters

`manifest`: The manifest to get e.g. `android_pvrtc.manifest`

---

_Example Response (shortened)_

```json
{
    "ClientVersion": 3302067,
    "BuildUrl": "CL_3302067/Android_PVRTC",
    "files": [
        {
            "filename": "WorldExplorers_pakchunk1000CL_3302067.manifest",
            "uniqueFilename": "WorldExplorers_pakchunk1000CL_3302067.manifest",
            "length": 935,
            "URL": "WorldExplorers_pakchunk1000CL_3302067.manifest",
            "hash": "679B16502124122A736F30A2190C1114D479D110",
            "hash256": "4C4C9245E345FA8D541ADA71595C7BBF23F2547FC6B1408FF9A39FF34277CD6C"
        }
    ]
}
```
