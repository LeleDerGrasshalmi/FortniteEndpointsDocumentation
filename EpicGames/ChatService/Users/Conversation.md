## Chat Service - Users: Conversation

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/users/:accountId/conversations/:conversationId \
Method: GET \
Auth Required: Yes (Account Auth)

## Path Parameters

`namespace`: e.g. `_` <br/>
`accountId`: Your AccountId <br/>
`conversationId`: The Conversation Id

## Query Parameters

`includeLastMessage`: `true` to include `lastMessage`

---

_Example Response (Group)_

```json
{
  "conversationId": "07c0ExampleGroupId0001",
  "title": "Docs Test",
  "type": "group",
  "createdBy": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60",
  "dateCreated": "2026-10-14T22:29:51.034Z",
  "active": true,
  "isActive": true,
  "isReportable": false,
  "members": ["c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60"],
  "invited": ["94b1569506b04f9f8557af611e8c5e47"],
  "joinedAt": "2026-10-14T22:29:51.132Z",
  "unreadCount": 0,
  "hasMoreUnread": false,
  "lastMessage": {
    "type": "social.chat.v1.NEW_MESSAGE",
    "metadata": {
      "Pub": "<jwt>",
      "Sig": "<base64 ed25519 signature>",
      "TmV": "2"
    },
    "msgId": "07c0ExampleMessageId11",
    "senderId": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60",
    "createdAt": "2026-10-14T22:29:51.323Z",
    "isReportable": false,
    "message": {
      "body": "<base64 payload>"
    }
  },
  "lastActivityId": "07c0ExampleMessageId10"
}
```

`message.body` is the signed payload, see [Message Signing](../README.md#message-signing)
