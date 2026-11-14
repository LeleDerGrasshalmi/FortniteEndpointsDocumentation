## Chat Service - Users: Conversations

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/users/:accountId/conversations \
Method: GET \
Auth Required: Yes (Account Auth)

## Path Parameters

`namespace`: e.g. `_` <br/>
`accountId`: Your AccountId

## Query Parameters

`includeLastMessage`: `true` to include `lastMessage` <br/>
`sortBy`: `lastActivity` <br/>
`limit`: Page size, e.g. `20`

---

_Example Response_

```json
{
  "conversations": [
    {
      "conversationId": "GBD2ExampleConversationId00001",
      "type": "dm",
      "createdBy": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60",
      "dateCreated": "2026-10-14T18:08:25.244Z",
      "active": true,
      "isActive": true,
      "isReportable": false,
      "members": ["c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60", "94b1569506b04f9f8557af611e8c5e47"],
      "unreadCount": 0,
      "hasMoreUnread": false,
      "lastMessage": {
        "type": "social.chat.v1.NEW_MESSAGE",
        "metadata": {
          "Pub": "<jwt>",
          "Sig": "<base64 ed25519 signature>",
          "TmV": "2"
        },
        "msgId": "07bzExampleMessageId01",
        "senderId": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60",
        "createdAt": "2026-10-14T18:08:25.369Z",
        "isReportable": false,
        "message": {
          "body": "<base64 payload>"
        }
      },
      "lastActivityId": "07bzExampleMessageId01"
    }
  ]
}
```
