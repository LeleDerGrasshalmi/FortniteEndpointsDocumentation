## Party Service V2 - Update Party Member Metadata

URL: https://api.epicgames.dev/epic/party/internal/v2/parties/:partyId/members/:accountId/meta \
Method: PATCH \
Auth Required: Yes (Account Auth)

```json
{
  "revision": 0,
  "update": {
    "active_voice_connection": "3a9c51fffe7d2e48-00000001-0007c2d4-5b1e9f0a7c3d2b6e-4f8a1c2d",
    "platform_name": "Windows",
    "product_name": "Epic Games Launcher"
  },
  "connection": {
    "id": "3a9c51fffe7d2e48-00000001-0007c2d4-5b1e9f0a7c3d2b6e-4f8a1c2d",
    "deployment_id": "_",
    "active_in_party_voice_room": true
  }
}
```

## Path Parameters

`partyId`: Party Id <br/>
`accountId`: Your AccountId

## Parameters

`revision`: Your current member `revision` <br/>
`update`: An object with the member meta keys you want updated <br/>
`connection.id`: Your Connection ID (EOS Connect Stomp) <br/>
`connection.deployment_id`: The deployment id, e.g. `_` <br/>
`connection.active_in_party_voice_room`: Whether this connection is in the party voice room

---

_Example Response_

```json
{
  "account_id": "94b1569506b04f9f8557af611e8c5e47",
  "meta": {
    "platform_name": "Windows",
    "product_name": "Epic Games Launcher",
    "active_voice_connection": "3a9c51fffe7d2e48-00000001-0007c2d4-5b1e9f0a7c3d2b6e-4f8a1c2d"
  },
  "revision": 1,
  "updated_at": "2026-10-14T16:53:45.378Z",
  "joined_at": "2026-10-14T16:53:45.116Z",
  "suspended": false,
  "connection": {
    "id": "3a9c51fffe7d2e48-00000001-0007c2d4-5b1e9f0a7c3d2b6e-4f8a1c2d",
    "deployment_id": "_",
    "connected_at": "2026-10-14T16:53:45.116Z",
    "updated_at": "2026-10-14T16:53:45.378Z",
    "is_first_party": true,
    "meta": {
      "osName": "Windows",
      "platformName": "egs",
      "productName": "Epic Games Launcher"
    },
    "active_in_party_voice_room": true
  }
}
```
