## Chat Service - Users: DM Conversation

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/users/:accountId/conversations/dm/:friendId \
Method: GET \
Auth Required: Yes (Account Auth)

## Path Parameters

`namespace`: e.g. `_` <br/>
`accountId`: Your AccountId <br/>
`friendId`: The other AccountId

## Query Parameters

`includeLastMessage`: `true` to include `lastMessage`

---

_Example Response_

```json
{
  "conversationId": "GBD2ExampleConversationId00001",
  "type": "dm",
  "createdBy": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60",
  "dateCreated": "2026-10-14T18:08:25.244Z",
  "active": true,
  "isActive": true,
  "isReportable": false,
  "members": ["c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60", "94b1569506b04f9f8557af611e8c5e47"],
  "unreadCount": 1,
  "hasMoreUnread": false,
  "lastMessage": {
    "type": "social.chat.v1.NEW_MESSAGE",
    "metadata": {
      "Pub": "<jwt>",
      "Sig": "<base64 ed25519 signature>",
      "TmV": "2"
    },
    "msgId": "07c0ExampleMessageId04",
    "senderId": "94b1569506b04f9f8557af611e8c5e47",
    "createdAt": "2026-10-14T22:05:43.889Z",
    "isReportable": false,
    "message": {
      "body": "<base64 payload>"
    }
  },
  "lastActivityId": "07c0ExampleMessageId04"
}
```

_Example Response (No DM yet)_

```json
{
  "type": "dm",
  "active": true,
  "isActive": true,
  "isReportable": false
}
```
