## IP-Data Service - Check Region

URL: https://ip-data-service-prod.ecbc.live.use1a.on.epicgames.com/region/check \
Method: POST \
Auth Required: Yes (`ipdata:region READ`)

```json
{
  "allow_on_error": false,
  "type": "continent",
  "limits": {
    "EU": "Res=656"
  },
  "content_id": "AF9yLAAsklQALFTy"
}
```

## Parameters

`allow_on_error`: Boolean <br/>
`type`: Type to check <br/>
`limits`: Unknown <br/>
`content_id`: Base64 of the following (Example below):

- `continent.geoname_id`
- `country.geoname_id`
- `subdivisions.geoname_id` (All Elements)

_Example Region lookup data (shortened)_

```json
{
  "continent": {
    "geoname_id": 6255148
  },
  "country": {
    "geoname_id": 2921044
  },
  "subdivisions": [
    {
      "geoname_id": 2905330
    }
  ]
}
```

All the numbers should be written as an Int32 Numbers as binary using **Big Endian**. <br/>
Then we would have the following Value (here showcased as hex): `00 5F 72 2C 00 2C 92 54 00 2C 54 F2` <br/>
As Base64: `AF9yLAAsklQALFTy`

---

_Example Response_

```json
{
  "content_id": "AF9yLAAsklQALFTy",
  "allowed": true,
  "resolved": true,
  "limit": "Res=656"
}
```
