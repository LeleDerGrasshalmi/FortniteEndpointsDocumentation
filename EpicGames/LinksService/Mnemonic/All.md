## Links Service - Mnemonic All

URL: https://links-public-service-live.ol.epicgames.com/links/api/:namespace/mnemonic/:mnemonic/all \
Method: GET \
Auth Required: Yes (`links:{namespace} READ`)

## Path Parameters

`namespace`: For Fortnite it's 'fn' <br/>
`mnemonic`: e.g. `1111-1111-1111` for FN Creative Island

---

_Example Response_

```json
[
  {
    "namespace": "fn",
    "accountId": "epic",
    "creatorName": "Epic",
    "mnemonic": "playlist_trios",
    "linkType": "BR:Playlist",
    "metadata": {
      "parent_set": "set_br_playlists",
      "favorite_override": "experience_br",
      "alt_title": {
        "de": "Trio",
        "ru": "Трио",
        "ko": "트리오",
        "zh-hant": "三人",
        "pt-BR": "Trios",
        "zh-hans": "三人",
        "it": "Terzetti",
        "fr": "Trios",
        "es": "Trio ",
        "ar": "ثلاثي",
        "vi": "3v3",
        "th": "ทรีโอ้",
        "ja": "トリオ",
        "id": "Trio",
        "pl": "Trójki",
        "es-419": "En trío",
        "tr": "Üçlü"
      },
      "play_history_override": "experience_br",
      "parent_experience": "experience_br",
      "image_url": "https://cdn2.unrealengine.com/solosize-1920-1920x1080-741c5c77900f.jpg",
      "product_tag": "Product.BR.Build.Trio",
      "image_urls": {
        "url_s": "https://cdn2.unrealengine.com/triossize-480-480x270-e63ad326c057.jpg",
        "url_xs": "https://cdn2.unrealengine.com/triossize-256-256x144-20919940fe51.jpg",
        "url_m": "https://cdn2.unrealengine.com/triossize-640-640x360-ab65f15eb2e0.jpg",
        "url": "https://cdn2.unrealengine.com/solosize-1920-1920x1080-741c5c77900f.jpg"
      },
      "dynamicXp": {
        "uniqueGameVersion": 95,
        "calibrationPhase": "LiveXp"
      },
      "title": "Trio",
      "matchmaking": {
        "override_playlist": "playlist_trios"
      },
      "video_vuid": "taqdZkWyokbCyEFWld"
    },
    "version": 95,
    "active": true,
    "disabled": false,
    "created": "2021-10-01T00:56:45.053Z",
    "published": "2021-08-03T15:27:20.799Z",
    "updated": "2025-09-17T23:52:05.040Z",
    "descriptionTags": [],
    "moderationStatus": "Unmoderated"
  }
]
```
