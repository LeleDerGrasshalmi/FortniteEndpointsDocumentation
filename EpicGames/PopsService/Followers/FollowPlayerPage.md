## Player Overview Page Service: Follow Player Page

URL: https://pops-api-live-public.ogs.live.on.epicgames.com/followers/v1/:playerId <br/>
Method: PUT <br/>
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

*Example Response*: Status 204
