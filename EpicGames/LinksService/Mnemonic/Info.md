## Links Service - Mnemonic Info

URL: https://links-public-service-live.ol.epicgames.com/links/api/:namespace/mnemonic/:mnemonic \
Method: GET \
Auth Required: Yes (`links:{namespace} READ`)

## Path Parameters

`namespace`: For Fortnite it's 'fn' <br/>
`mnemonic`: e.g. `1111-1111-1111` for FN Creative Island

## Query Parameters

`type`: Mnemonic Type e.g. 'Creative:Island' or 'BR:Playlist' <br/>
`v`: Mnemonic Version to lookup, omit for latest <br/>
`includeActivationHistory`: Optional boolean to include the activation history

---

_Example Response_

```json
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
```

_Example Response (with activation history)_

```json
{
  "namespace": "fn",
  "accountId": "epic",
  "creatorName": "Epic",
  "mnemonic": "set_delmar_mrs_ranked",
  "linkType": "ModeSet",
  "metadata": {
    "extra_video_vuids": ["ae921b8f-ceea-428b-8b4b-c83f2f77fd8f"],
    "blog_category": "rocket-racing",
    "frontend_plugin": "DelMarFrontendMinimal",
    "image_urls": {
      "url_s": "https://cdn2.unrealengine.com/rr-playlisttile-2-480-480x270-b5a5fdfb40ba.jpg",
      "url_xs": "https://cdn2.unrealengine.com/rr-playlisttile-2-256-256x144-53baf8c6588e.jpg",
      "url_m": "https://cdn2.unrealengine.com/rocketracing-launchtile-640-640x360-17247961b9e5.jpg",
      "url": "https://cdn2.unrealengine.com/rocketracing-launchtile-1920x1080-4c78a6359538.jpg"
    },
    "title": "Rocket Racing",
    "locale": "en",
    "video_vuid": "nKaFcQbEhacuiRdfFD",
    "matchmakingV2": {
      "ratingType": "delmar-competitive",
      "isRanked": true
    },
    "activated_public_date": "2023-12-08T13:00:00.000Z",
    "matchmaking_plugins": [
      "DelMarMatchmakingErrors",
      "DelMarReadyUpErrors",
      "DelMarGracefulUpgrade",
      "DelMarMatchmakingSettingsButton",
      "DelMarTrackSelectorUI",
      "DelMarFrontend"
    ],
    "product_tag": "Product.DelMar",
    "ratings": {
      "rating_received_time": "2023-12-02T12:29:33.028Z",
      "boards": {}
    },
    "ccu_source_links": ["playlist_delmar_ranked_root", "..."],
    "web_slug": "rocket-racing",
    "corresponding_sets": {
      "unranked": "set_delmar_casual"
    },
    "lobby_background_image_urls": {
      "url": "https://cdn2.unrealengine.com/delmar-lobby-notext-4096x2048-1fcb8f7605ac.jpg"
    },
    "image_url": "https://cdn2.unrealengine.com/rocketracing-launchtile-1920x1080-4c78a6359538.jpg",
    "genre_labels": ["Driving"],
    "unlockConditions": {
      "allOf": {
        "conditions": []
      },
      "partyEligibility": "EVERYONE"
    },
    "sub_link_codes": ["playlist_delmar_ranked_root", "..."],
    "tagline": "Start your engines then drift, fly, and boost your way to the finish in a rocket-powered car! Climb the ranks and test your skills in Ranked or pull up to Casual Racing and enjoy the thrill of racing without high stakes. Want to race against the clock? Drop into Speed Run and put your best time on the leaderboard.",
    "extra_image_urls": [
      {
        "url_s": "https://cdn2.unrealengine.com/cdn-uploader-rr_gameplay_screenshot_pov2_-lg-1920x1080-ead95a8e.jpg",
        "url_m": "https://cdn2.unrealengine.com/cdn-uploader-rr_gameplay_screenshot_pov2_-lg-1920x1080-ead95a8e.jpg",
        "url": "https://cdn2.unrealengine.com/cdn-uploader-rr_gameplay_screenshot_pov2_-lg-1920x1080-ead95a8e.jpg"
      }
    ],
    "category_labels": ["Driving"],
    "default_sub_link_code": "playlist_delmar_ranked_root"
  },
  "version": 1,
  "active": true,
  "disabled": false,
  "created": "2023-11-30T19:04:39.696Z",
  "published": "2023-11-30T19:04:39.696Z",
  "updated": "2025-12-16T23:22:53.161Z",
  "descriptionTags": [],
  "moderationStatus": "Approved",
  "lastActivatedDate": "2023-12-02T22:56:20.965Z",
  "discoveryIntent": "PUBLIC",
  "activationHistory": [
    {
      "mnemonic": "set_delmar_mrs_ranked",
      "version": 1,
      "activated": "2023-12-02T22:56:20.967Z"
    }
  ],
  "linkCategory": "ROCKET RACING"
}
```
