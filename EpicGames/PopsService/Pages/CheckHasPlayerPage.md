## Player Overview Page Service: Check Has Player Page

URL: https://pops-api-live-public.ogs.live.on.epicgames.com/page/v1/:pagePlayerId/check <br/>
Method: GET <br/>
Auth Required: Yes (`pops:playerpage READ`)

## Path Parameters

`pagePlayerId`: Page Player's Account Id

---

*Example Response (has page)*

```json
{
  "hasPage": true
}
```

*Example Response (has no page)*

```json
{
  "hasPage": false
}
```
