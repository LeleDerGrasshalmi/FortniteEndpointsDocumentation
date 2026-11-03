## Chat Service - Conversations: Leave Conversation

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/conversations/:conversationId/members/:accountId \
Method: DELETE \
Auth Required: Yes (Account Auth)

## Path Parameters

`namespace`: e.g. `_` <br/>
`conversationId`: The Conversation Id <br/>
`accountId`: Your AccountId

---

_Example Response_: Status 204

Leaving a deactivated conversation (see [Conversation](./Conversation.md)) also returns Status 204.

_Example Response (After leaving)_

Requests from that account on the conversation (metadata, messages, invites, leaving again) return 404.

```json
{
  "messageVars": [],
  "errorMessage": "Conversation 07c0ExampleGroupId0001 in namespace _ not found",
  "errorCode": "errors.com.epicgames.social.chat.conversation_not_found",
  "correlationId": "8e4c2a1b-3d5f-4a7b-9c0d-2e1f3a4b5c6d",
  "numericErrorCode": 40401,
  "responseStatus": 404,
  "intent": "prod",
  "originatingService": "chat-service-api-prod"
}
```
