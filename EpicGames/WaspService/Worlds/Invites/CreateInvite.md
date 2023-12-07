## Wasp Service - Create World Invite

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/ownedBy/:accountId \
Method: POST \
Auth Required: Yes (`wasp:{namespaceId}:invite CREATE`)

```json
{
  "accountId": ""
}
```

## Path Parameters

`namespaceId`: Check [Readme](../../README.md) <br/>
`worldId` The World Id from the [worlds list](../AccountAccessibleWorld.md)

## Parameters

The payload is not complete, therefore this request will just return an "Server Error".

`accountId`: Account Id of the account to invite, must match `^[a-zA-Z0-9_./!-]{1,128}$` (regex)
