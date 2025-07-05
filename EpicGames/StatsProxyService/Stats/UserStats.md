## 統計プロキシ-ユーザー統計

URL: https://statsproxy-public-service-live.ol.epicgames.com/statsproxy/api/statsv2/account/:accountId \
メソッド: GET \
認証の有無: Yes (`fortnite:stats READ`)

## パスパラメータ

`accountId`: アカウント

## クエリパラメータ

`startTime`: 既定:0,カスタム時間枠に設定可能 <br/>
`endTime`: カスタム時間枠に設定可能<br/>

---

__レスポンスの例__

```json
{
  "startTime": 0,
  "endTime": 9223372036854775807,
  "stats": {
    "br_playersoutlived_keyboardmouse_m0_playlist_melt_duos": 32,
    "br_placetop12_keyboardmouse_m0_playlist_bots_defaultduo": 25,
    "br_placetop5_keyboardmouse_m0_playlist_deimos_duo_winter": 2,
    "br_score_keyboardmouse_m0_playlist_habanerosolo": 472
  },
  "accountId": "d1d7a59146f14b4b9f76a5cb00a38f41"
}
```

__レスポンスの例(統計OFFのアカウントの場合)__:status204
