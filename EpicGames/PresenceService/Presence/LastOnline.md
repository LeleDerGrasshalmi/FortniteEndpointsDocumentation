## Presence Service - Last Online

URL: https://presence-public-service-prod.ol.epicgames.com/presence/api/v1/:namespace/:accountId/last-online \
Method: GET \
Auth Required: Yes (`presence:{namespace}:{accountId}:lastOnline`)

## Path Parameters
`accountId`: Your AccountId
`namespace`: e.g. `_` or `Fortnite`

---

_Example Response_

```json
{
  "192b217e425b429f8b52c2004dbbaa85": [
    {
      "namespace": "Fortnite",
      "last_online": "2026-03-01T19:49:34.782Z"
    }
  ],
  "040fc7da57354ec4bd1e437ae6cc1d82": [
    {
      "namespace": "Fortnite",
      "last_online": "2026-02-26T18:08:43.901Z"
    }
  ]
}
```