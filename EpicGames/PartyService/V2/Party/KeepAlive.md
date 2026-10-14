## Party Service V2 - Keep Alive

URL: https://api.epicgames.dev/epic/party/internal/v2/parties/:partyId/members/:accountId/keep-alive \
Method: POST \
Auth Required: Yes (Account Auth)

## Path Parameters

`partyId`: The Party ID <br/>
`accountId`: Your AccountId

---

_Example Response_

```json
{
  "account_id": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60",
  "meta": {},
  "revision": 0,
  "updated_at": "2026-10-14T17:57:26.758Z",
  "joined_at": "2026-10-14T17:57:26.758Z",
  "suspended": false
}
```
