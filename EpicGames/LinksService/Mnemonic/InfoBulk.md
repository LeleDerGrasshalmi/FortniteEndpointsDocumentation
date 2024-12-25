## Links Service - Mnemonic Info (Bulk)

URL: https://links-public-service-live.ol.epicgames.com/links/api/:namespace/mnemonic \
Method: POST \
Auth Required: Yes (`links:{namespace} READ`)

```json
[
  {
    "mnemonic": "playlist_defaultsolo",
    "type": "",
    "filter": false,
    "v": ""
  }
]
```

## Path Parameters

`namespace`: For Fortnite it's 'fn'

## Parameters

`mnemonic`: e.g. `1111-1111-1111` for FN Creative Island <br/>
`type`: Mnemonic Type e.g. 'Creative:Island' or 'BR:Playlist' <br/>
`filter`: Unknown <br/>
`v`: Mnemonic Version to lookup, leave empty for latest

## Query Parameters

`ignoreFailures`: Optional (boolean), if the request should **not** throw an Error when any Lookup failed (should usually be set to true)

---

_Example Response (shortened)_

```json
[
  {
    "namespace": "fn",
    "accountId": "epic",
    "creatorName": "Epic",
    "mnemonic": "playlist_defaultsolo",
    "linkType": "BR:Playlist",
    "metadata": {
      "parent_set": "set_br_playlists",
      "favorite_override": "set_br_playlists",
      "play_history_override": "set_br_playlists",
      "alt_title": {
        "de": "Solo"
      },
      "image_url": "https://cdn2.unrealengine.com/solosize-1920-1920x1080-741c5c77900f.jpg",
      "product_tag": "Product.BR.Build.Solo",
      "image_urls": {
        "url_s": "https://cdn2.unrealengine.com/solosize-480-480x270-bd71a8aecb8f.jpg",
        "url_xs": "https://cdn2.unrealengine.com/solosize-256-256x144-9e4ba5075e53.jpg",
        "url_m": "https://cdn2.unrealengine.com/solosize-640-640x360-0062a2e4e8b4.jpg",
        "url": "https://cdn2.unrealengine.com/solosize-1920-1920x1080-741c5c77900f.jpg"
      },
      "dynamicXp": {
        "uniqueGameVersion": 95,
        "calibrationPhase": "LiveXp"
      },
      "matchmaking": {
        "override_playlist": "playlist_defaultsolo"
      },
      "video_vuid": "taqdZkWyokbCyEFWld",
      "title": "Solo"
    },
    "version": 95,
    "active": true,
    "disabled": false,
    "created": "2021-10-01T00:56:43.870Z",
    "published": "2021-08-03T15:27:17.540Z",
    "descriptionTags": [],
    "moderationStatus": "Unmoderated"
  },
  {
    "namespace": "fn",
    "accountId": "epic",
    "creatorName": "Epic",
    "mnemonic": "playlist_defaultduo",
    "linkType": "BR:Playlist",
    "metadata": {
      "parent_set": "set_br_playlists",
      "favorite_override": "set_br_playlists",
      "play_history_override": "set_br_playlists",
      "alt_title": {
        "de": "Duo"
      },
      "image_url": "https://cdn2.unrealengine.com/duossize-1920-1920x1080-284f117a184a.jpg",
      "product_tag": "Product.BR.Build.Duo",
      "image_urls": {
        "url_s": "https://cdn2.unrealengine.com/duossize-480-480x270-f7ab641d8d9c.jpg",
        "url_xs": "https://cdn2.unrealengine.com/duossize-256-256x144-6291155853c9.jpg",
        "url_m": "https://cdn2.unrealengine.com/duossize-640-640x360-9cd7be7aba4c.jpg",
        "url": "https://cdn2.unrealengine.com/duossize-1920-1920x1080-284f117a184a.jpg"
      },
      "dynamicXp": {
        "uniqueGameVersion": 95,
        "calibrationPhase": "LiveXp"
      },
      "matchmaking": {
        "override_playlist": "playlist_defaultduo"
      },
      "video_vuid": "taqdZkWyokbCyEFWld",
      "title": "Duo"
    },
    "version": 95,
    "active": true,
    "disabled": false,
    "created": "2021-10-01T00:56:46.389Z",
    "published": "2021-08-03T15:27:17.523Z",
    "descriptionTags": [],
    "moderationStatus": "Unmoderated"
  }
]
```
