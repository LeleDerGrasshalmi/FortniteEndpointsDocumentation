## Chat Service - Conversations: Update Invite Status

Accepting moves the account from `invited` to `members` of the group conversation.

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/conversations/:conversationId/invites/:accountId \
Method: PATCH \
Auth Required: Yes (Account Auth)

```json
{
  "status": "accepted"
}
```

## Path Parameters

`namespace`: e.g. `_` <br/>
`conversationId`: The Conversation Id <br/>
`accountId`: Your AccountId

## Parameters

`status`: `accepted` or `rejected`

## Query Parameters

`setMessagesToRead`: `true` / `false`

---

_Example Response_

```json
{}
```

Returns `errors.com.epicgames.social.chat.conversation_not_found` (404) if the conversation no longer exists, see [Leave Conversation](./LeaveConversation.md)

_Example Response (After rejecting)_

`rejected` also returns `{}`. Afterwards requests from that account on the conversation return 404:

```json
{
  "messageVars": [],
  "errorMessage": "Conversation 07c0ExampleGroupId0004 in namespace _ not found",
  "errorCode": "errors.com.epicgames.social.chat.conversation_not_found",
  "correlationId": "2d7a9c4e-1b3f-4e8a-9d6c-5f0b1a2e3c4d",
  "numericErrorCode": 40401,
  "responseStatus": 404,
  "intent": "prod",
  "originatingService": "chat-service-api-prod"
}
```
