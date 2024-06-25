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
    "lobby_background_image_urls": {
      "url": "https://cdn2.unrealengine.com/delmarlobby-4096x2048-d68bbc69fdab.jpg"
    },
    "frontend_plugin": "DelMarFrontend",
    "image_url": "https://cdn2.unrealengine.com/rocketracing-launchtile-1920x1080-4c78a6359538.jpg",
    "title": "Rocket Racing",
    "locale": "en",
    "product_tag": "Product.DelMar",
    "tagline": "From the developers of Rocket League comes Rocket Racing, a supersonic arcade racer that lets you drift, fly, and boost with your friends through an ever-growing selection of tracks. It's Season Zero, hop into a rocket-powered car and put your skills to the test!"
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
  ]
}
```
