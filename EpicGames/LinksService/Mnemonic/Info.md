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
    "favorite_override": "set_br_playlists",
    "play_history_override": "set_br_playlists",
    "alt_title": {
      "de": "Trio",
      "ru": "Трио",
      "ko": "트리오",
      "pt-BR": "Trios",
      "zh-hans": "三人",
      "en": "Trio",
      "it": "Terzetti",
      "fr": "Trios",
      "zh-CN": "",
      "es": "Tríos",
      "es-MX": "En trío",
      "zh": "",
      "ar": "ثلاثي",
      "zh-Hant": "",
      "ja": "トリオ",
      "pl": "Trójki",
      "es-419": "En trío",
      "tr": "Üçlü"
    },
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
    "matchmaking": {
      "override_playlist": "playlist_trios"
    },
    "video_vuid": "taqdZkWyokbCyEFWld",
    "title": "Trio"
  },
  "version": 95,
  "active": true,
  "disabled": false,
  "created": "2021-10-01T00:56:45.053Z",
  "published": "2021-08-03T15:27:20.799Z",
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
    "lobby_background_image_urls": {
      "url": "https://cdn2.unrealengine.com/delmar-lobby-notext-4096x2048-1fcb8f7605ac.jpg"
    },
    "blog_category": "rocket-racing",
    "frontend_plugin": "DelMarFrontend",
    "image_url": "https://cdn2.unrealengine.com/rocketracing-launchtile-1920x1080-4c78a6359538.jpg",
    "image_urls": {
      "url_s": "https://cdn2.unrealengine.com/rr-playlisttile-2-480-480x270-b5a5fdfb40ba.jpg",
      "url_xs": "https://cdn2.unrealengine.com/rr-playlisttile-2-256-256x144-53baf8c6588e.jpg",
      "url_m": "https://cdn2.unrealengine.com/rocketracing-launchtile-640-640x360-17247961b9e5.jpg",
      "url": "https://cdn2.unrealengine.com/rocketracing-launchtile-1920x1080-4c78a6359538.jpg"
    },
    "title": "Rocket Racing",
    "locale": "en",
    "video_vuid": "nKaFcQbEhacuiRdfFD",
    "unlockConditions": {
      "allOf": {
        "conditions": []
      },
      "partyEligibility": "EVERYONE"
    },
    "sub_link_codes": [
      "playlist_delmar_ranked_root",
      "playlist_delmar_bronze06_nux"
    ],
    "matchmakingV2": {
      "ratingType": "delmar-competitive",
      "isRanked": true
    },
    "alt_title": {
      "de": "Rocket Racing"
    },
    "alt_tagline": {
      "de": "Starte deine Motoren und drifte, fliege und rase in einem Auto mit Raketenantrieb ins Ziel! Steige in den Rängen auf und zeige dein Können in „Ranked“ oder genieße ein Zwangloses Rennen ohne den ganzen Druck. Du möchtest ein Rennen gegen die Zeit fahren? Dann schau beim Zeitfahren vorbei und schaffe es auf die Bestenliste."
    },
    "matchmaking_plugins": [
      "DelMarMatchmakingErrors",
      "DelMarGracefulUpgrade",
      "DelMarMatchmakingSettingsButton"
    ],
    "product_tag": "Product.DelMar",
    "ratings": {
      "rating_received_time": "2023-12-02T12:29:33.028Z",
      "boards": {
        "USK": {
          "descriptors": [],
          "rating_overridden": false,
          "rating": "USK_AGE_12",
          "initial_rating": "USK_AGE_12",
          "interactive_elements": [
            "IE_UsersInteract",
            "IE_InGamePurchases_v7_1"
          ]
        }
      }
    },
    "ccu_source_links": [
      "playlist_delmar_ranked_root",
      "playlist_delmar_bronze06_nux",
      "playlist_delmar_bronze10_nux"
    ],
    "fallback_links": {
      "graceful": "playlist_delmar_racing_root"
    },
    "tagline": "Start your engines then drift, fly, and boost your way to the finish in a rocket-powered car! Climb the ranks and test your skills in Ranked or pull up to Casual Racing and enjoy the thrill of racing without high stakes. Want to race against the clock? Drop into Speed Run and put your best time on the leaderboard.",
    "extra_image_urls": [
      {
        "url_s": "https://fortnite-vod.akamaized.net/qpdchKarjFnwpdEnYj/39723da0-b595-4f92-9a98-c35ebb75bae3/rr_gameplay_screenshot_pov1_1920x1080-sm.jpg",
        "url_m": "https://fortnite-vod.akamaized.net/qpdchKarjFnwpdEnYj/39723da0-b595-4f92-9a98-c35ebb75bae3/rr_gameplay_screenshot_pov1_1920x1080-md.jpg",
        "url": "https://fortnite-vod.akamaized.net/qpdchKarjFnwpdEnYj/39723da0-b595-4f92-9a98-c35ebb75bae3/rr_gameplay_screenshot_pov1_1920x1080-lg.jpg"
      }
    ],
    "square_image_urls": {
      "url": "https://cdn2.unrealengine.com/en-rr-launch-discovery-tile-square-sq-480x480-cf65dc7c8a8b.jpg"
    },
    "corresponding_sets": {
      "unranked": "set_delmar_casual"
    },
    "default_sub_link_code": "playlist_delmar_ranked_root"
  },
  "version": 1,
  "active": true,
  "disabled": false,
  "created": "2023-11-30T19:04:39.696Z",
  "published": "2023-11-30T19:04:39.696Z",
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
