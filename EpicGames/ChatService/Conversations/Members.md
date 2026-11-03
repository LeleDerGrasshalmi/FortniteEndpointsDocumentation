## Chat Service - Conversations: Members

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/conversations/:conversationId/members \
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
  "members": ["c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60", "94b1569506b04f9f8557af611e8c5e47"]
}
```

_Example Response (Group)_

`invited` is only present while invites are pending

```json
{
  "conversationId": "07c0ExampleGroupId0002",
  "members": ["94b1569506b04f9f8557af611e8c5e47", "c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60"],
  "invited": ["5e2d8c1b9a7f4e3d8c6b2a1f0e9d7c3b"]
}
```
