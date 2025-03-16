## Player Overview Page Service: Follow Player Page

URL: https://pops-api-live-public.ogs.live.on.epicgames.com/followers/v1/:playerId \
Method: PUT \
Auth Required: Yes (`pops:follow:{accountId} UPDATE`)

```json
{
  "playerIdToFollow": "epic"
}
```

## Path Parameters

`playerId`: Your Account Id

## Parameters

`playerIdToFollow`: Page Player's Account Id

---

_Example Response_: Status 204
