## FN Service - User Stats (V1)

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/stats/accountId/:accountId/bulk/window/:windowId \
Method: GET \
Auth Required: Yes

## Path Parameters

`accountId`: The Target Account Id <br/>
`windowId`: 'alltime' / 'weekly'

> Has been removed ages ago.

---

_Example Response_

```json
[
  {
    "name": "br_score_pc_m0_p10",
    "value": 1190306,
    "window": "alltime",
    "ownerType": 1
  },
  {
    "name": "br_score_pc_m0_p2",
    "value": 1142038,
    "window": "alltime",
    "ownerType": 1
  },
  {
    "name": "br_kills_pc_m0_p2",
    "value": 26746,
    "window": "alltime",
    "ownerType": 1
  },
  {
    "name": "br_matchesplayed_pc_m0_p2",
    "value": 3458,
    "window": "alltime",
    "ownerType": 1
  },
  {
    "name": "br_kills_pc_m0_p9",
    "value": 10133,
    "window": "alltime",
    "ownerType": 1
  },
  {
    "name": "br_minutesplayed_pc_m0_p2",
    "value": 24386,
    "window": "alltime",
    "ownerType": 1
  }
]
```
