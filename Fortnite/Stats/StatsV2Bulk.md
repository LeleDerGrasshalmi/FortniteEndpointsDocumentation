## Fortnite - User Stats (BULK)

URL: https://statsproxy-public-service-live.ol.epicgames.com/statsproxy/api/statsv2/query \
Method: POST \
Auth Required: Yes

```json
{
  "appId": "Fortnite",
  "startDate": 0,
  "endDate": 9223372036854775807,
  "owners": ["accountId"],
  "stats": ["s22_social_bp_level"]
}
```

**owners**: Array of every Account Id to query \
**stats**: Array of every Stat to query
