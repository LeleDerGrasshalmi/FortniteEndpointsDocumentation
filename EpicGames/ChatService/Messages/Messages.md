## Chat Service - Messages: Conversation Messages

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/conversations/:conversationId/messages \
Method: GET \
Auth Required: Yes (Account Auth)

## Path Parameters

`namespace`: e.g. `_` <br/>
`conversationId`: The Conversation Id

## Query Parameters

`requestingAccountId`: Your AccountId <br/>
`limit`: Page size, e.g. `30`

---

_Example Response_

```json
{
  "page": [
    {
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
    {
      "type": "social.chat.v1.NEW_MESSAGE",
      "metadata": {
        "Pub": "<jwt>",
        "Sig": "<base64 ed25519 signature>",
        "TmV": "2"
      },
      "msgId": "07bzExampleMessageId02",
      "senderId": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60",
      "createdAt": "2026-10-14T18:08:25.783Z",
      "isReportable": false,
      "message": {
        "body": "<base64 payload>"
      }
    },
    {
      "type": "social.chat.v1.REPORTABILITY_CHANGE",
      "system": true,
      "msgId": "07bzExampleMessageId03",
      "createdAt": "2026-10-14T18:08:25.337Z",
      "payload": {
        "isReportable": false
      }
    }
  ],
  "hasNextPage": false
}
```

`message.body` is the signed payload, see [Message Signing](../README.md#message-signing)

_Example Response (Group)_

```json
{
  "page": [
    {
      "type": "social.chat.v1.MEMBERS_JOIN",
      "system": true,
      "msgId": "07c0ExampleMessageId15",
      "createdAt": "2026-10-14T22:29:57.732Z",
      "payload": {
        "members": ["94b1569506b04f9f8557af611e8c5e47"],
        "isReportable": false
      }
    },
    {
      "type": "social.chat.v1.TITLE_CHANGE",
      "system": true,
      "msgId": "07c0ExampleMessageId14",
      "createdAt": "2026-10-14T22:29:51.575Z",
      "payload": {
        "accountId": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60",
        "title": "Docs Test Renamed",
        "previousTitle": "Docs Test",
        "isReportable": false
      }
    },
    {
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
    {
      "type": "social.chat.v1.REPORTABILITY_CHANGE",
      "system": true,
      "msgId": "07c0ExampleMessageId13",
      "createdAt": "2026-10-14T22:29:51.197Z",
      "payload": {
        "isReportable": false
      }
    },
    {
      "type": "social.chat.v1.NEW_INVITE",
      "system": true,
      "msgId": "07c0ExampleMessageId12",
      "createdAt": "2026-10-14T22:29:51.173Z",
      "payload": {
        "isReportable": false,
        "inviter": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60",
        "invited": ["94b1569506b04f9f8557af611e8c5e47"]
      }
    }
  ],
  "hasNextPage": false
}
```

System entries (`"system": true`) and their `payload`:

`social.chat.v1.NEW_INVITE`: `isReportable`, `inviter`, `invited` <br/>
`social.chat.v1.REPORTABILITY_CHANGE`: `isReportable` <br/>
`social.chat.v1.MEMBERS_JOIN`: `members`, `isReportable` <br/>
`social.chat.v1.TITLE_CHANGE`: `accountId`, `title`, `previousTitle`, `isReportable`

Returns `errors.com.epicgames.social.chat.conversation_not_found` (404) after leaving the conversation, see [Leave Conversation](../Conversations/LeaveConversation.md)
