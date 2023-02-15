## Links Service - Mnemonic Info (Bulk)

URL: https://links-public-service-live.ol.epicgames.com/links/api/:namespace/mnemonic?ignoreFailures=true \
Method: GET \
Auth Required: Yes (`links:{namespace} READ`)

```json
[
  {
    "mnemonic": "",
    "type": "",
    "filter": false,
    "v": ""
  }
]
```

## Path Parameter

`namespace`: For Fortnite it's 'fn'

## Parameter

`mnemonic`: e.g. `1111-1111-1111` for FN Creative Island <br/>
`type`: Mnemonic Type? e.g. 'Creative:Island' or 'BR:Playlist' <br/>
`filter`: Unknown <br/>
`v`: Mnemonic Version to lookup, leave empty for latest <br/>

## Query Parameter

`ignoreFailures`: Optional boolean, if the request should **not** throw an Error when any Lookup failed
