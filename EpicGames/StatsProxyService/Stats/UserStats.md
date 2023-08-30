## Stats Proxy: User Stats

URL: https://statsproxy-public-service-live.ol.epicgames.com/statsproxy/api/statsv2/account/:accountId \
Method: GET \
Auth Required: Yes (`fortnite:stats READ`)

## Path Parameters

`accountId`: target User Account Id

## Query Parameters

`startTime`: optional, 0 (for alltime) or set for custom time-window <br/>
`endTime`: optional, 9223372036854775807 (for alltime) or set for custom time-window <br/>

---

_Example Response_

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

_Example Response (Private Stats)_: Status 204
