## Links Service - Mnemonic Info with related Mnemonic Infos

URL: https://links-public-service-live.ol.epicgames.com/links/api/:namespace/mnemonic/:mnemonic/related \
Method: GET \
Auth Required: Yes (`links:{namespace} READ`)

## Path Parameter

`namespace`: For Fortnite it's 'fn' <br/>
`mnemonic`: e.g. `1111-1111-1111` for FN Creative Island or `playlist_trios` for normal Trios

---

Example Response (shortened)

```json
{
  "parentLinks": [
    {
      "namespace": "fn",
      "accountId": "epic",
      "creatorName": "Epic",
      "mnemonic": "set_br_playlists",
      "linkType": "ModeSet",
      "metadata": {
        "alt_title": {
          "de": "Battle Royale",
          "ru": "Королевская битва",
          "ko": "배틀로얄",
          "pt-BR": "Battle Royale",
          "it": "Battaglia reale",
          "fr": "Battle Royale",
          "zh-CN": "",
          "es": "Battle Royale",
          "es-MX": "Batalla campal",
          "zh": "",
          "ar": "باتل رويال",
          "zh-Hant": "",
          "ja": "バトルロイヤル",
          "pl": "Battle Royale",
          "es-419": "Batalla campal",
          "tr": "Battle Royale"
        },
        "alt_tagline": {
          "de": "Überlebe allein in einer Schlacht bis auf den letzten Spieler.",
          "ru": "Отправляйтесь на битву в одиночку и переживите всех соперников.",
          "ko": "죽느냐 사느냐... 혼자서 싸우는 서바이벌 혈투!",
          "pt-BR": "Entre sozinho em uma batalha para ser o último sobrevivente.",
          "it": "Combatti in solitaria fino a diventare l'ultimo superstite.",
          "fr": "Combattez en solitaire et soyez le dernier survivant.",
          "zh-CN": "",
          "es": "Entra en solitario en un combate para ser el último en pie.",
          "es-MX": "Entra por tu cuenta a un combate y pelea hasta que solo quedes tú en pie.",
          "zh": "",
          "ar": "خُض المعركة بمفردك لتصبح آخر من يتبقى من اللاعبين.",
          "zh-Hant": "",
          "ja": "単身でバトルに飛び込み、最後の1人になるまで生き残れ。",
          "pl": "Walcz samotnie w bitwie do ostatniego.",
          "es-419": "Entra por tu cuenta a un combate y pelea hasta que solo quedes tú en pie.",
          "tr": "Savaşa tek başına gir ve hayatta kalan son kişi ol."
        },
        "image_url": "https://cdn2.unrealengine.com/nocturnal-br-1920-1920x1080-c17716b1607d.png",
        "image_urls": {
          "url_s": "https://cdn2.unrealengine.com/nocturnal-br-480-480x270-55a14d4c57cd.png",
          "url_xs": "https://cdn2.unrealengine.com/nocturnal-br-256-256x144-8f3ba6805684.png",
          "url_m": "https://cdn2.unrealengine.com/nocturnal-br-640-640x360-0ae0f6b8a8ee.png",
          "url": "https://cdn2.unrealengine.com/nocturnal-br-1920-1920x1080-c17716b1607d.png"
        },
        "tagline": "The battle is building! \r\n Drop into the Battle Royale. Loot, build, explore, and fight in a game of 100 players competing to be the last one standing.",
        "title": "Battle Royale",
        "locale": "en",
        "video_vuid": "taqdZkWyokbCyEFWld",
        "sub_link_codes": [
          "playlist_defaultsolo",
          "playlist_defaultduo",
          "playlist_trios",
          "playlist_defaultsquad"
        ],
        "default_sub_link_code": "playlist_defaultsquad"
      },
      "version": 1,
      "active": true,
      "disabled": false,
      "created": "2022-06-30T17:57:54.767Z",
      "published": "2022-06-30T17:57:54.767Z",
      "descriptionTags": [],
      "moderationStatus": "Unmoderated",
      "lastActivatedDate": "2022-06-30T17:57:54.770Z"
    }
  ],
  "links": {
    "playlist_defaultduo": {
      "namespace": "fn",
      "accountId": "epic",
      "creatorName": "Epic",
      "mnemonic": "playlist_defaultduo",
      "linkType": "BR:Playlist",
      "metadata": {},
      "version": 95,
      "active": true,
      "disabled": false,
      "created": "2021-10-01T00:56:46.389Z",
      "published": "2021-08-03T15:27:17.523Z",
      "descriptionTags": [],
      "moderationStatus": "Unmoderated"
    },
    "playlist_trios": {
      "namespace": "fn",
      "accountId": "epic",
      "creatorName": "Epic",
      "mnemonic": "playlist_trios",
      "linkType": "BR:Playlist",
      "metadata": {
        "parent_set": "set_br_playlists",
        "favorite_override": "set_br_playlists",
        "play_history_override": "set_br_playlists",
        "image_url": "https://cdn2.unrealengine.com/s24-trios-1920-1920x1080-3e751867870b.jpg",
        "image_urls": {
          "url_s": "https://cdn2.unrealengine.com/s24-trios-480-480x270-42df252e6002.jpg",
          "url_xs": "https://cdn2.unrealengine.com/s24-trios-256-256x144-0585c93c17fe.jpg",
          "url_m": "https://cdn2.unrealengine.com/s24-trios-640-640x360-242337935fac.jpg",
          "url": "https://cdn2.unrealengine.com/s24-trios-1920-1920x1080-3e751867870b.jpg"
        },
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
      "descriptionTags": [],
      "moderationStatus": "Unmoderated"
    },
    "playlist_defaultsolo": {
      "namespace": "fn",
      "accountId": "epic",
      "creatorName": "Epic",
      "mnemonic": "playlist_defaultsolo",
      "linkType": "BR:Playlist",
      "metadata": {},
      "version": 95,
      "active": true,
      "disabled": false,
      "created": "2021-10-01T00:56:43.870Z",
      "published": "2021-08-03T15:27:17.540Z",
      "descriptionTags": [],
      "moderationStatus": "Unmoderated"
    },
    "playlist_defaultsquad": {
      "namespace": "fn",
      "accountId": "epic",
      "creatorName": "Epic",
      "mnemonic": "playlist_defaultsquad",
      "linkType": "BR:Playlist",
      "metadata": {},
      "version": 95,
      "active": true,
      "disabled": false,
      "created": "2021-10-01T00:56:42.938Z",
      "published": "2021-08-03T15:27:17.566Z",
      "descriptionTags": [],
      "moderationStatus": "Unmoderated"
    }
  }
}
```
