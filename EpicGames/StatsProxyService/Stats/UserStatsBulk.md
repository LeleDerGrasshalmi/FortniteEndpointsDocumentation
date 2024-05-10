## Stats Proxy: User Stats (Bulk)

URL: https://statsproxy-public-service-live.ol.epicgames.com/statsproxy/api/statsv2/query \
Method: POST \
Auth Required: Yes (`fortnite:stats READ`)

```json
{
  "appId": "Fortnite",
  "startDate": 0,
  "endDate": 9223372036854775807,
  "owners": ["accountId"],
  "stats": ["s22_social_bp_level"]
}
```

## Parameters

`appId`: only `Fortnite` is known to be valid <br/>
`startDate`: 0 (for alltime) or set for custom time-window <br/>
`endDate`: 9223372036854775807 (for alltime) or set for custom time-window <br/>
`owners`: the Account Ids to query Stats from <br/>
`stats`: Optional, incase you only want to query specific Stat Ids <br/>

## Query Parameters

`category`: Optional, if used `stats` in the body should not be used, allows fetching a Collection, valid values:

- `collection_fish`
- `collection_character`

---

> When the Stats are private there won't be an Entry for the given Account

_Example Response for Collection Data_

```json
[
  {
    "startTime": 0,
    "endTime": 9223372036854775807,
    "stats": {
      "br_collection_fish_gas_purple_length_s16": 51421,
      "br_collection_fish_zeropoint_tidal_length_s21": 77466,
      "br_collection_fish_jellyfish_purple_length_s17": 46166,
      "br_collection_fish_lesseffectiveflopper_blue_length_s17": 18923,
      "br_collection_fish_jellyfish_pink_length_s19": 47579,
      "br_collection_fish_flameyfish_black_length_s16": 53010,
      "br_collection_fish_rift_volcanic_length_s15": 62649,
      "br_collection_fish_flameyfish_black_length_s17": 39315,
      "br_collection_fish_flopper_blue_length_s19": 47376,
      "br_collection_fish_shieldfish.lightblue__length_s20": 41965
    },
    "accountId": "d1d7a59146f14b4b9f76a5cb00a38f41"
  }
]
```

_Example Response for Stats Data with only the `s23_social_bp_level` Stat_

```json
[
  {
    "startTime": 0,
    "endTime": 9223372036854775807,
    "stats": {
      "s23_social_bp_level": 2274
    },
    "accountId": "d1d7a59146f14b4b9f76a5cb00a38f41"
  }
]
```
