## Party Service V2 - Get Party

URL: https://api.epicgames.dev/epic/party/internal/v2/parties/:partyId \
Method: GET \
Auth Required: Yes (Account Auth)

## Path Parameters

`partyId`: The Party ID

---

_Example Response_

```json
{
  "id": "2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f",
  "party_lead": "94b1569506b04f9f8557af611e8c5e47",
  "created_at": "2026-10-14T17:58:53.823Z",
  "updated_at": "2026-10-14T17:58:54.568Z",
  "config": {
    "joinability": "INVITE_ONLY",
    "max_size": 16
  },
  "meta": {
    "created_by": "94b1569506b04f9f8557af611e8c5e47"
  },
  "revision": 1,
  "chat_conversation_id": "ep-2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f",
  "is_reportable": true,
  "members": [
    {
      "account_id": "94b1569506b04f9f8557af611e8c5e47",
      "meta": {
        "platform_name": "Windows",
        "product_name": "Epic Games Launcher",
        "active_voice_connection": "3a9c51fffe7d2e48-00000001-0007c2d4-5b1e9f0a7c3d2b6e-4f8a1c2d"
      },
      "revision": 1,
      "updated_at": "2026-10-14T17:58:54.114Z",
      "joined_at": "2026-10-14T17:58:53.829Z",
      "suspended": false,
      "connections": [
        {
          "id": "3a9c51fffe7d2e48-00000001-0007c2d4-5b1e9f0a7c3d2b6e-4f8a1c2d",
          "deployment_id": "_",
          "connected_at": "2026-10-14T17:58:53.829Z",
          "updated_at": "2026-10-14T17:58:54.114Z",
          "is_first_party": true,
          "meta": {
            "osName": "Windows",
            "platformName": "egs",
            "productName": "Epic Games Launcher"
          },
          "active_in_party_voice_room": true
        }
      ]
    },
    {
      "account_id": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60",
      "meta": {
        "platform_name": "Windows",
        "product_name": "Epic Games Launcher",
        "active_voice_connection": "6b4e20fffe8a1d57-00000001-05a3e9c1-7d2f4b6a8c0e1f35-2c9a7e4b"
      },
      "revision": 1,
      "updated_at": "2026-10-14T17:58:54.537Z",
      "joined_at": "2026-10-14T17:58:54.316Z",
      "suspended": false,
      "connections": [
        {
          "id": "6b4e20fffe8a1d57-00000001-05a3e9c1-7d2f4b6a8c0e1f35-2c9a7e4b",
          "deployment_id": "_",
          "connected_at": "2026-10-14T17:58:54.315Z",
          "updated_at": "2026-10-14T17:58:54.537Z",
          "is_first_party": true,
          "meta": {
            "osName": "Windows",
            "platformName": "egs",
            "productName": "Epic Games Launcher"
          },
          "active_in_party_voice_room": true
        }
      ]
    }
  ]
}
```

_Example Response (Party not found)_

```json
{
  "errorCode": "errors.com.epicgames.social.party.party_not_found",
  "errorMessage": "Party [2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f] does not exist.",
  "messageVars": [
    "2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f"
  ],
  "numericErrorCode": 51002,
  "originatingService": "party-v2",
  "intent": "prod"
}
```
