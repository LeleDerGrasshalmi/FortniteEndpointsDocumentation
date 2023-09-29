## Id Web - Check DisplayName Duplicate

URL: https://www.epicgames.com/id/api/account/displayName/validate \
Method: POST \
Auth Required: Yes

```json
{
  "displayName": "lele stw moment"
}
```

---

_Example Response (Used)_

```json
{
  "errorCode": "errors.com.epicgames.account.duplicate_display_name",
  "message": "Sorry, this display name is already in use.",
  "metadata": {},
  "correlationId": "08494c00-ff19-11ed-8544-3b67346e1363"
}
```

_Example Response(unused)_: `Status 200` (But no Content)
