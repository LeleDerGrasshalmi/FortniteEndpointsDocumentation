## Chat Service - Conversations: Add Members

Invites more accounts to a group conversation.

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/conversations/:conversationId/members \
Method: POST \
Auth Required: Yes (Account Auth)

```json
{
  "members": ["5e2d8c1b9a7f4e3d8c6b2a1f0e9d7c3b"]
}
```

## Path Parameters

`namespace`: e.g. `_` <br/>
`conversationId`: The Conversation Id

## Parameters

`members`: AccountIds to invite

## Query Parameters

`requestingAccountId`: Your AccountId <br/>
`invite`: `true`

---

_Example Response_

```json
{
  "invited": ["5e2d8c1b9a7f4e3d8c6b2a1f0e9d7c3b"],
  "notInvited": []
}
```
