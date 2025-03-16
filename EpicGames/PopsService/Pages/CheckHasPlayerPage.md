## Player Overview Page Service: Check Has Player Page

URL: https://pops-api-live-public.ogs.live.on.epicgames.com/page/v1/:pagePlayerId/check \
Method: GET \
Auth Required: Yes (`pops:playerpage READ`)

## Path Parameters

`pagePlayerId`: Page Player's Account Id

---

_Example Response (has page)_

```json
{
  "hasPage": true
}
```

_Example Response (has no page)_

```json
{
  "hasPage": false
}
```
