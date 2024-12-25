## Links Service - Mnemonic Info with related Mnemonics

URL: https://links-public-service-live.ol.epicgames.com/links/api/:namespace/mnemonic/:mnemonic/related \
Method: GET \
Auth Required: Yes (`links:{namespace} READ`)

## Path Parameters

`namespace`: For Fortnite it's 'fn' <br/>
`mnemonic`: e.g. `1111-1111-1111` for FN Creative Island or `playlist_trios` for normal Trios

## Query Parameters

`v`: Mnemonic Version to lookup, leave empty for latest

---

_Example Response (shortened)_

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
        "blog_category": "battle-royale",
        "image_url": "https://cdn2.unrealengine.com/fnbr-33-00-c6s1-discoverplaylist-tiles-br-1920x1080v2-1920x1080-3f75c79fb1f4.jpg",
        "image_urls": {
          "url_s": "https://cdn2.unrealengine.com/fnbr-33-00-c6s1-discoverplaylist-tiles-br-480x270v2-480x270-8c8fd9f4f1f4.jpg",
          "url_xs": "https://cdn2.unrealengine.com/fnbr-33-00-c6s1-discoverplaylist-tiles-br-256x144v2-256x144-4be9bd0ddcf1.jpg",
          "url_m": "https://cdn2.unrealengine.com/fnbr-33-00-c6s1-discoverplaylist-tiles-br--640x360v2-640x360-951fc1f7f397.jpg",
          "url": "https://cdn2.unrealengine.com/fnbr-33-00-c6s1-discoverplaylist-tiles-br-1920x1080v2-1920x1080-3f75c79fb1f4.jpg"
        },
        "title": "Battle Royale",
        "locale": "en",
        "video_vuid": "BPmqJrpZmlEdIOGook",
        "sub_link_codes": [
          "playlist_defaultsolo",
          "playlist_defaultduo",
          "playlist_trios",
          "playlist_defaultsquad"
        ],
        "alt_title": {
          "de": "Battle Royale"
        },
        "alt_tagline": {
          "de": "Baut euch euren Weg zum Sieg! Stürzt euch in Battle Royale. Sammelt Beute, baut, erkundet und kämpft in einer Schlacht von 100 Spielern, bis nur noch einer übrig ist."
        },
        "ratings": {
          "rating_received_time": "2023-11-16T00:00:00.575Z",
          "boards": {
            "USK": {
              "descriptors": ["USK_FantasyGewalt_v9_0"],
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
        "product_tag": "Product.BR.Build",
        "fallback_links": {
          "graceful": "playlist_respawn_24_alt"
        },
        "tagline": "• Hitscan Weapons: All traditional weapons in Battle Royale Chapter 6 will be hitscan.\n• New Movement: Ledge Jump, Roll Landing, Wall Kick and Wall Scramble.\n• Magical Abilities: Teleport with the Void Oni Mask, sprint faster with the Typhoon Blade, and more!\n\nThe battle is building! Drop into the Battle Royale. Loot, build, explore, and fight in a game of 100 players competing to be the last one standing.",
        "extra_image_urls": [
          {
            "url_s": "https://cdn2.unrealengine.com/fnbr-33-00-c6s1-quail-screenshot6-motd-1920x1080-640x360-1733032628647-640x360-54421599af14.jpg",
            "url_m": "https://cdn2.unrealengine.com/fnbr-33-00-c6s1-quail-screenshot6-motd-1920x1080-640x360-1733032628647-640x360-54421599af14.jpg",
            "url": "https://cdn2.unrealengine.com/fnbr-33-00-c6s1-quail-screenshot6-motd-1920x1080-1920x1080-fdfc69ed3564.jpg"
          }
        ],
        "square_image_urls": {
          "url": "https://cdn2.unrealengine.com/fnbr-33-00-c6s1-discoverplaylist-tiles-br-480x480v2-480x480-1e4439c70a3a.jpg"
        },
        "corresponding_sets": {
          "ranked": "set_habanero_playlists"
        },
        "default_sub_link_code": "playlist_defaultsquad"
      },
      "version": 1,
      "active": true,
      "disabled": false,
      "created": "2022-06-30T17:57:54.767Z",
      "published": "2022-06-30T17:57:54.767Z",
      "descriptionTags": [],
      "moderationStatus": "Approved",
      "lastActivatedDate": "2022-06-30T17:57:54.770Z",
      "discoveryIntent": "PUBLIC"
    },
    {
      "namespace": "fn",
      "accountId": "epic",
      "creatorName": "Epic",
      "mnemonic": "set_habanero_playlists",
      "linkType": "ModeSet",
      "metadata": {
        "blog_category": "ranked",
        "image_url": "https://static-assets-prod.epicgames.com/fn/static/1p/27ranked-br-modetiles-ranked-br-1920x1080-1920x1080-e664cc196e16_s.jpg",
        "image_urls": {
          "url_s": "https://static-assets-prod.epicgames.com/fn/static/1p/Ranked_BR_480_s.jpg",
          "url_xs": "https://static-assets-prod.epicgames.com/fn/static/1p/Ranked_BR_256_s.jpg",
          "url_m": "https://static-assets-prod.epicgames.com/fn/static/1p/Ranked_BR_640_s.jpg",
          "url": "https://static-assets-prod.epicgames.com/fn/static/1p/27ranked-br-modetiles-ranked-br-1920x1080-1920x1080-e664cc196e16_s.jpg"
        },
        "locale": "en",
        "title": "Ranked Battle Royale",
        "video_vuid": "iYrWMWYEnnantjNdRv",
        "unlockConditions": {
          "allOf": {
            "conditions": [
              {
                "id": "habanero_unlocked",
                "type": "profile"
              }
            ]
          },
          "partyEligibility": "EVERYONE"
        },
        "sub_link_codes": [
          "playlist_habanerosolo",
          "playlist_habaneroduo",
          "playlist_habanerotrio",
          "playlist_habanerosquad"
        ],
        "matchmakingV2": {
          "ratingType": "ranked-br",
          "isRanked": true
        },
        "alt_title": {
          "de": "Ranked Battle Royale"
        },
        "alt_tagline": {
          "de": "Wie das klassische Battle Royale, nur mit noch mehr Nervenkitzel! Tritt gegen andere Spieler mit ähnlichem Rang an. Beweise deine Fähigkeiten, schließe Herausforderungen für Belohnungen ab, und steig in der Rangliste auf!"
        },
        "ratings": {
          "rating_received_time": "2023-11-16T00:00:00.575Z",
          "boards": {
            "USK": {
              "descriptors": ["USK_FantasyGewalt_v9_0"],
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
        "product_tag": "Product.BR.Habanero.Build",
        "fallback_links": {
          "graceful": "playlist_respawn_24_alt"
        },
        "tagline": "Just like classic Battle Royale, with a little more to play for!\nBattle it out against other players of similar rank. Show off your skills, complete challenges for rewards, and climb the ranks.",
        "square_image_urls": {
          "url": "https://cdn2.unrealengine.com/28-discoverytiles-updated-ranked-br-sq-480x480-ba3ec852a65d.jpg"
        },
        "corresponding_sets": {
          "unranked": "set_br_playlists"
        },
        "default_sub_link_code": "playlist_habanerosquad"
      },
      "version": 1,
      "active": true,
      "disabled": false,
      "created": "2023-04-11T18:32:46.910Z",
      "published": "2023-04-11T18:32:46.910Z",
      "descriptionTags": [],
      "moderationStatus": "Approved",
      "lastActivatedDate": "2023-04-11T18:32:46.913Z",
      "discoveryIntent": "PUBLIC"
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
        "alt_title": {
          "de": "Trio"
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
    },
    "playlist_habaneroduo": {
      "namespace": "fn",
      "accountId": "epic",
      "creatorName": "Epic",
      "mnemonic": "playlist_habaneroduo",
      "linkType": "BR:Playlist",
      "metadata": {},
      "version": 1,
      "active": true,
      "disabled": false,
      "created": "2023-03-16T00:09:06.826Z",
      "published": "2023-03-16T00:09:06.826Z",
      "descriptionTags": [],
      "moderationStatus": "Unmoderated",
      "lastActivatedDate": "2023-03-16T00:09:06.828Z",
      "discoveryIntent": "PUBLIC"
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
    "playlist_habanerosolo": {
      "namespace": "fn",
      "accountId": "epic",
      "creatorName": "Epic",
      "mnemonic": "playlist_habanerosolo",
      "linkType": "BR:Playlist",
      "metadata": {},
      "version": 1,
      "active": true,
      "disabled": false,
      "created": "2023-03-28T19:48:00.449Z",
      "published": "2023-03-28T19:48:00.449Z",
      "descriptionTags": [],
      "moderationStatus": "Unmoderated",
      "lastActivatedDate": "2023-03-28T19:48:00.451Z",
      "discoveryIntent": "PUBLIC"
    },
    "playlist_habanerotrio": {
      "namespace": "fn",
      "accountId": "epic",
      "creatorName": "Epic",
      "mnemonic": "playlist_habanerotrio",
      "linkType": "BR:Playlist",
      "metadata": {},
      "version": 1,
      "active": true,
      "disabled": false,
      "created": "2023-03-28T19:48:00.390Z",
      "published": "2023-03-28T19:48:00.390Z",
      "descriptionTags": [],
      "moderationStatus": "Unmoderated",
      "lastActivatedDate": "2023-03-28T19:48:00.392Z",
      "discoveryIntent": "PUBLIC"
    },
    "playlist_respawn_24_alt": {
      "namespace": "fn",
      "accountId": "epic",
      "creatorName": "Epic",
      "mnemonic": "playlist_respawn_24_alt",
      "linkType": "BR:Playlist",
      "metadata": {},
      "version": 95,
      "active": true,
      "disabled": false,
      "created": "2021-10-01T00:56:43.052Z",
      "published": "2021-08-03T15:27:20.393Z",
      "descriptionTags": [],
      "moderationStatus": "Approved",
      "discoveryIntent": "PUBLIC"
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
    },
    "playlist_habanerosquad": {
      "namespace": "fn",
      "accountId": "epic",
      "creatorName": "Epic",
      "mnemonic": "playlist_habanerosquad",
      "linkType": "BR:Playlist",
      "metadata": {},
      "version": 1,
      "active": true,
      "disabled": false,
      "created": "2023-03-28T19:48:01.293Z",
      "published": "2023-03-28T19:48:01.293Z",
      "descriptionTags": [],
      "moderationStatus": "Unmoderated",
      "lastActivatedDate": "2023-03-28T19:48:01.295Z",
      "discoveryIntent": "PUBLIC"
    }
  }
}
```
