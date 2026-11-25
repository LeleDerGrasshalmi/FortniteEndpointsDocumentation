## Friends Service - Set External Source Settings

URL: https://friends-public-service-prod06.ol.epicgames.com/friends/api/v1/:accountId/settings/externalSources/:source <br/>
Method: PUT <br/>
Auth Required: Yes (`friends:{accountId} UPDATE`)

```json
{
  "doNotShowLinkingProposal": false
}
```

## Path Parameters

`accountId`: Your Account Id <br/>
`source`: See [Readme](README.md)

## Parameters

`doNotShowLinkingProposal`: (bool), if the Linking Popup should not be shown again

---

*Example Response*

```json
{
  "doNotShowLinkingProposal": false
}
```
