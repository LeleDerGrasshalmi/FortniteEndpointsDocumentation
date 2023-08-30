## Artifact Delivery Service - Patch

URL: https://artifact-delivery-public-service-prod.beee.live.use1a.on.epicgames.com/artifact-delivery/api/public/v1/delivery/account/:accountId/patch \
Method: POST \
Auth Required: Yes (`delivery:public:patch:{accountId} READ`)

```json
{
  "signedTicket": "eyJzaGFyZElkIjoiZWdzIiwiYXJ0aWZhY3RJZCI6IkZvcnRuaXRlIiwiZ3JhbnRBY2Nlc3NUb0RlcGVuZGVuY2llcyI6ZmFsc2UsImV4cGlyZXNBdCI6IjIwMjMtMDgtMzBUMTg6Mjk6MjdaIiwiYWNjb3VudElkIjoiOTRiMTU2OTUwNmIwNGY5Zjg1NTdhZjYxMWU4YzVlNDciLCJiaW5hcnlWZXJzaW9uIjoiKytGb3J0bml0ZStSZWxlYXNlLTI2LjAwLUNMLTI3NDI0NzkwLVdpbmRvd3MifQ==.Y2ZlMTRhNGQxMmQyMWY2ODAzOTc4NmY2MmY1YWViMjYzMDQxNGQyZjE0ODRjZWQxOGIyNTdiOTI2MmNlOWFmMA=="
}
```

## Path Parameters

`accountId`: Your AccountId

## Parameters

`signedTicket`: The Signed Ticket that is obtained using the [Launcher Service Ticket API](/EpicGames/LauncherService/Assets/V2/Ticket/CreateTicket.md)

> Payload not fully known
