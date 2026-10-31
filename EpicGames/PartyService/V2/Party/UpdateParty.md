## Party Service V2 - Update Party Config

URL: https://api.epicgames.dev/epic/party/internal/v2/parties/:partyId \
Method: PATCH \
Auth Required: Yes (Account Auth)

```json
{
  "config": {
    "joinability": "OPEN",
    "max_size": 16
  },
  "revision": 0
}
```

## Path Parameters

`partyId`: Party Id

## Parameters

`config.joinability`: `OPEN` or `INVITE_ONLY` <br/>
`config.max_size`: Max party size, `16` <br/>
`revision`: The current party `revision`

---

_Example Response_

```json
{
  "id": "2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f",
  "party_lead": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60",
  "created_at": "2026-10-14T17:57:26.752Z",
  "updated_at": "2026-10-14T17:57:27.163Z",
  "config": {
    "joinability": "OPEN",
    "max_size": 16
  },
  "meta": {
    "created_by": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60"
  },
  "revision": 1,
  "chat_conversation_id": "ep-2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f",
  "is_reportable": false
}
```
