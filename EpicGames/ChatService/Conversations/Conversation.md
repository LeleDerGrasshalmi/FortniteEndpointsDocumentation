## Chat Service - Conversations: Conversation

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/conversations/:conversationId \
Method: GET \
Auth Required: Yes (Account Auth)

## Path Parameters

`namespace`: e.g. `_` <br/>
`conversationId`: The Conversation Id

## Query Parameters

`accountId`: Your AccountId

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
  "members": ["c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60", "94b1569506b04f9f8557af611e8c5e47"]
}
```

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
  "invited": ["94b1569506b04f9f8557af611e8c5e47"]
}
```

_Example Response (Deactivated group)_

A group with only one member left and no pending invites is deactivated.

```json
{
  "conversationId": "07c0ExampleGroupId0003",
  "title": "Docs Reject Test",
  "type": "group",
  "createdBy": "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60",
  "dateCreated": "2026-10-14T22:52:13.936Z",
  "active": false,
  "isActive": false,
  "inactiveReason": "insufficient_members",
  "isReportable": false,
  "members": ["c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60"]
}
```
