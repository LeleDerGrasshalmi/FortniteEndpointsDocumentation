## Party Service V2 - Get Voice Room Connection

URL: https://api.epicgames.dev/epic/party/internal/v2/parties/:partyId/members/:accountId/conferences/connection \
Method: POST \
Auth Required: Yes (Account Auth)

## Path Parameters

`partyId`: The Party ID <br/>
`accountId`: Your AccountId

---

_Example Response_

```json
{
  "providers": {
    "rtcp": {
      "participant_token": "REDACTED",
      "client_base_url": "wss://signaling-service-prod.use2.live.rtcp.on.epicgames.com/ws?ms=wss://10.0.12.34:8443/6c1e2f3a-4b5d-4e6f-8a9b-0c1d2e3f4a5b&p=epicparty&t=MTAuMC4xMi4zNHwxMjM0NTY3OA.3KnMtEhf9pnxsRtWn1QSq3d0j0wPmuJ7oN_ruEZsWW4",
      "room_name": "pv2-2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f"
    }
  }
}
```
