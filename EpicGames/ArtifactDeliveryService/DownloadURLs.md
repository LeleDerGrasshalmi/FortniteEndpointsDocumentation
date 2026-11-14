## Artifact Delivery Service - Generate Download URLs

URL: https://artifact-delivery-public-service-prod.beee.live.use1a.on.epicgames.com/artifact-delivery/api/public/v1/delivery/account/:accountId/downloadurls \
Method: POST \
Auth Required: Yes (`delivery:public:downloadurls:{accountId} READ`)

```json
{
  "signedTicket": "eyJzaGFyZElkIjoiZWdzIiwiYXJ0aWZhY3RJZCI6IkZvcnRuaXRlIiwiZ3JhbnRBY2Nlc3NUb0RlcGVuZGVuY2llcyI6ZmFsc2UsImV4cGlyZXNBdCI6IjIwMjMtMDUtMTBUMTU6NDk6MjlaIiwiYWNjb3VudElkIjoiOTRiMTU2OTUwNmIwNGY5Zjg1NTdhZjYxMWU4YzVlNDciLCJiaW5hcnlWZXJzaW9uIjoiKytGb3J0bml0ZStSZWxlYXNlLTI0LjMwLUNMLTI1MzQ3MzgyLVdpbmRvd3MifQ==.YmRkOGMyNmY5OTVkNzQzNThlMjIwNjI5MTljOWU0MjJkMjgxNWQ5NjE4MmVlM2E3MmM3NjA4N2EwZjg4MWIxZQ==",
  "chunkIds": ["4F2230B528691E80_55B266154D97BA6252E59B88E70EED90"]
}
```

## Path Parameters

`accountId`: Your AccountId

## Parameters

`signedTicket`: The Signed Ticket that is obtained using the [Launcher Service Ticket API](/EpicGames/LauncherService/Assets/V2/Ticket/CreateTicket.md) <br/>
`chunkIds`: All Chunk Ids you want to generate Download URLs for

---

_Example Response_

```json
{
  "4F2230B528691E80_55B266154D97BA6252E59B88E70EED90": "https://download.epicgames.com/Builds/Fortnite/CloudDir/4F2230B528691E80_55B266154D97BA6252E59B88E70EED90?Policy=eyJTdGF0ZW1lbnQiOiBbeyJSZXNvdXJjZSI6IipCdWlsZHMvRm9ydG5pdGUvQ2xvdWREaXIvKiIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTY5MjEyNDgxM30sIklwQWRkcmVzcyI6eyJBV1M6U291cmNlSXAiOiIwLjAuMC4wLzAifX19XX0_&Signature=JJygeDaYRLoKpTiPpqzQ47KQQgVoILWLZOIDIhFgJbhJPrB5H8~mUIbrHReErjBYIVkoff33hUX3xCMSPdoYalWqB34qlNoM0QUF6WiGo6iRb497BT85pH0GtJyUngFMtNU-Nm31fcas8F09aEqw5Mqf3GDwzafm9cqGt05bm4abN3lCDB6dq5D7zx0woQpR~bX0GQNzXvpqBNNbLd1RIBwpS01mrCRfQmYtBaiSU4SLRXVj~X8Pu4fgCdlpn~gqYenrThP~DIROpaEvWMo~6MIyoKt7TCxbAmz12-~G6DzhGaJseIeEV1JlDtPqqQCYdXT5ait8BAEkE-TqMkbeWA__&Key-Pair-Id=APKAI5CNFPJPTPYZISXQ"
}
```

As of November 2026 a bare `<hash>_<guid>` chunk id is refused; `chunkIds` must be the chunk path relative to the build folder, e.g. `ChunksV4/99/AD4912FCD4E970C4_72E1EAE145AD588528C1549EE40CF696.chunk`. The Bearer token is the account access token (the ticket goes in the body).

_Example Response (November 2026)_

```json
{
  "ChunksV4/99/AD4912FCD4E970C4_72E1EAE145AD588528C1549EE40CF696.chunk": "https://egdownload.fastly-edge.com/Builds/Fortnite/CloudDir/ChunksV4/99/AD4912FCD4E970C4_72E1EAE145AD588528C1549EE40CF696.chunk"
}
```

_Example Response (chunk id not in path form)_

```json
{
  "errorCode": "errors.com.epicgames.artifactdelivery.unauthorized",
  "errorMessage": "Invalid chunkId found.",
  "intent": "prod",
  "messageVars": [],
  "numericErrorCode": 1002,
  "originatingService": "artifact-delivery-service-springboot"
}
```

Without `signedTicket`: 400 `errors.com.epicgames.artifactdelivery.bad_request` (`signedTicket cannot be null.`), with an invalid one: `Invalid signedTicket.`.
