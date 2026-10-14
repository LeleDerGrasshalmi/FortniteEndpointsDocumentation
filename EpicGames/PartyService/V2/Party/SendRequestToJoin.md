## Party Service V2 - Send Request To Join

URL: https://api.epicgames.dev/epic/party/internal/v2/users/:friendId/joinRequests/:accountId \
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
  "requester_id": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60",
  "requester_dn": "ExampleAlt",
  "requester_pl": "",
  "requester_pl_dn": "",
  "requestee_id": "94b1569506b04f9f8557af611e8c5e47",
  "sent_at": "2026-10-14T18:05:34.267Z",
  "expires_at": "2026-10-14T19:05:34.267Z",
  "auto": false
}
```
