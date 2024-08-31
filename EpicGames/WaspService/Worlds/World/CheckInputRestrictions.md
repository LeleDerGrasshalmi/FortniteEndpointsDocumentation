## Wasp Service - Check Input Restrictions

URL: https://wasp-service-live-public.ogs.live.on.epicgames.com/api/v1/namespace/:namespaceId/worlds/world/:worldId/inputRestrictions/:restrictionId/check \
Method: POST \
Auth Required: Yes (`wasp:{namespaceId}:world READ`)

```json
{
  "namedEntity": "WorldName",
  "proposedText": "hello github - whats up"
}
```

## Path Parameters

`namespaceId`: Check [Readme](../README.md) <br/>
`worldId` The World Id from the [worlds list](./AccountAccessibleWorld.md) or `NewWorld` when validating the name before creating a new world <br/>
`restrictionId`: `juno:ugcName` (must be url encoded), other strings may throw an error

## Parameters

`namedEntity`: `WorldName`, but can technically be any string,
`proposedText`: The text to validate

---

_Example Response_

```json
{
  "allowed": true
}
```
