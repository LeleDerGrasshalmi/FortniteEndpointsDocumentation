## Id Web - Send Analytics

URL: https://www.epicgames.com/id/api/analytics \
Method: POST \
Auth Required: Yes

```json
{
    "eventType": ""
}
```

## Parameters

`eventType`: The event/action currently in use to analyise. Valid: `EPIC_WEB_ANALYTICS_EVENT`, `MERGE_REDIRECT`, `EXT_AUTH_LOGIN_START`, `EXT_AUTH_LINK_START`, `EXT_AUTH_LOGIN_REDIRECT`

---

_Example Response (Successful)_: Status 200

```json
{
    "accountId": "6c5f78c40a31482f81ae5df98b950889",
    "trackingUuid": "58a9874d11ae4d619e1dd98a028229c4"
}
```
