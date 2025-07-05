## 統計プロキシ-ユーザー統計一括取得

URL: https://statsproxy-public-service-live.ol.epicgames.com/statsproxy/api/statsv2/query \
メソッド: POST \
認証の有無: Yes (`fortnite:stats READ`)

```json
{
  "appId": "Fortnite",
  "startDate": 0,
  "endDate": 9223372036854775807,
  "owners": ["accountId"],
  "stats": ["s22_social_bp_level"]
}
```

## パラメータ

`appId`:  `Fortnite`有効であるアカウント <br/>
`startDate`: カスタム時間枠に設定可能（デフォルト:0) <br/>
`endDate`:カスタム時間枠に設定可能（デフォルト：9223372036854775807） <br/>
`owners`: 統計をリクエストするアカウントID<br/>
`stats`: 特定の統計 ID のみを照会する場合のオプション <br/>

## クエリパラメータ

`category`:オプション:

- `collection_fish`
- `collection_character`

---

> 統計が公開されていないアカウントは204が返ってきます。

__コレクションデータに対するレスポンスの例__

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

__統計データのみの応答例__

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
