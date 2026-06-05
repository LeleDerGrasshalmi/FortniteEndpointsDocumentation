## Presence Service - Delete Presence

URL: https://presence-public-service-prod.ol.epicgames.com/presence/api/v1/:namespace/:accountId/presence/:connectionId \
Method: DELETE \
Auth Required: Yes (`presence:{namespace}:{accountId} DELETE`)

> Also available on eos under `https://api.epicgames.dev/epic/presence/v1/_:deploymentId_/:accountId/presence/:connectionId`

## Path Parameters

`accountId`: Your AccountId <br/>
`namespace`: The presence namespace, ex. `_` (launcher) or the deployment id (when using eos) <br/>
`connectionId`: Your Connection ID (XMPP/EOS Connect Stomp)
