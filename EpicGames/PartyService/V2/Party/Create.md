## Party Service V2 - Create Party

URL: https://api.epicgames.dev/epic/party/internal/v2/parties \
Method: POST \
Auth Required: Yes (Account Auth)

```json
{
  "config": {
    "joinability": "INVITE_ONLY",
    "max_size": 16
  },
  "meta": {
    "created_by": "94b1569506b04f9f8557af611e8c5e47"
  },
  "join_info": {
    "connection": {
      "id": "3a9c51fffe7d2e48-00000001-0007c2d4-5b1e9f0a7c3d2b6e-4f8a1c2d",
      "deployment_id": "_",
      "meta": {
        "osName": "Windows",
        "platformName": "egs",
        "productName": "Epic Games Launcher"
      }
    }
  }
}
```

## Parameters

`config.joinability`: `OPEN` or `INVITE_ONLY` <br/>
`config.max_size`: Max party size, `16` <br/>
`meta`: Party metadata <br/>
`join_info.connection.id`: Your Connection ID (EOS Connect Stomp) <br/>
`join_info.connection.deployment_id`: The deployment id, e.g. `_` <br/>
`join_info.connection.meta`: Connection metadata

---

_Example Response_

```json
{
  "id": "2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f",
  "party_lead": "94b1569506b04f9f8557af611e8c5e47",
  "created_at": "2026-10-14T16:53:45.111Z",
  "updated_at": "2026-10-14T16:53:45.111Z",
  "config": {
    "joinability": "INVITE_ONLY",
    "max_size": 16
  },
  "meta": {
    "created_by": "94b1569506b04f9f8557af611e8c5e47"
  },
  "revision": 0,
  "chat_conversation_id": "ep-2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f",
  "is_reportable": false,
  "members": [
    {
      "account_id": "94b1569506b04f9f8557af611e8c5e47",
      "meta": {},
      "revision": 0,
      "updated_at": "2026-10-14T16:53:45.116Z",
      "joined_at": "2026-10-14T16:53:45.116Z",
      "suspended": false,
      "connections": [
        {
          "id": "3a9c51fffe7d2e48-00000001-0007c2d4-5b1e9f0a7c3d2b6e-4f8a1c2d",
          "deployment_id": "_",
          "connected_at": "2026-10-14T16:53:45.116Z",
          "updated_at": "2026-10-14T16:53:45.111Z",
          "is_first_party": true,
          "meta": {
            "osName": "Windows",
            "platformName": "egs",
            "productName": "Epic Games Launcher"
          },
          "active_in_party_voice_room": false
        }
      ]
    }
  ]
}
```
