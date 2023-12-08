## Wasp Service - Create World Invite

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/invites/world/:worldId \
Method: POST \
Auth Required: Yes (`wasp:{namespaceId}:invite CREATE`)

```json
{
  "namespaceId": "fn",
  "worldId": "9f5f4fe52d594e0abe3bca3edf62899f",
  "accountId": "9d58d46c633f475e8f329d203b7a4198",
  "roleId": "juno_keyholder",
  "type": "PERSISTENT"
}
```

## Path Parameters

`namespaceId`: Check [Readme](../../README.md) <br/>
`worldId` The World Id from the [worlds list](../AccountAccessibleWorld.md)

## Parameters

`namespaceId`: Use the value from the path, but its ignored by the server <br/>
`worldId`: Use the value from the path, but its ignored by the server <br/>
`accountId`: Account Id of the account to invite, must match `^[a-zA-Z0-9_./!-]{1,128}$` (regex) <br/>
`roleId`: Only known supported value by this endpoint is `juno_keyholder` <br/>
`type`: Only known supported value by this endpoint is `PERSISTENT`

--

_Example Response_

`Status 201 (but no content)`
