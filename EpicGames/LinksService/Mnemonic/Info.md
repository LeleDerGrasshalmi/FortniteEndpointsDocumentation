## Links Service - Mnemonic Info

URL: https://links-public-service-live.ol.epicgames.com/links/api/:namespace/mnemonic/:mnemonic \
Method: GET \
Auth Required: Yes (`links:{namespace} READ`)

## Path Parameters

`namespace`: For Fortnite it's 'fn' <br/>
`mnemonic`: e.g. `1111-1111-1111` for FN Creative Island

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
