## Party Service V2 - Invite

URL: https://api.epicgames.dev/epic/party/internal/v2/users/:friendId/invites/:accountId \
Method: POST \
Auth Required: Yes (Account Auth)

## Path Parameters

`friendId`: Friend AccountId <br/>
`accountId`: Your AccountId

## Query Parameters

`auto`: `true` or `false`

---

_Example Response_

```json
{
  "party_id": "2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f",
  "sent_by": "94b1569506b04f9f8557af611e8c5e47",
  "auto": false,
  "meta": {},
  "sent_to": "5e2d8c1b9a7f4e3d8c6b2a1f0e9d7c3b",
  "sent_at": "2026-10-14T16:53:45.315Z",
  "updated_at": "2026-10-14T16:53:45.315Z",
  "expires_at": "2026-10-14T17:53:45.315Z"
}
```
