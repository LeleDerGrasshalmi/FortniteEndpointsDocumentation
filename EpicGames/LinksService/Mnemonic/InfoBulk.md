## Links Service - Mnemonic Info (Bulk)

URL: https://links-public-service-live.ol.epicgames.com/links/api/:namespace/mnemonic?ignoreFailures=true \
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

`ignoreFailures`: Optional (boolean), if the request should **not** throw an Error when any Lookup failed

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
    "metadata": {},
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
    "metadata": {},
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
