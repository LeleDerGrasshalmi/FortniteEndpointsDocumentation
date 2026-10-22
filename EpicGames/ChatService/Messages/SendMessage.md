## Chat Service - Messages: Send Message

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/conversations/:conversationId/messages \
Method: POST \
Auth Required: Yes (Account Auth)

```json
{
  "message": {
    "body": "<base64 payload>"
  },
  "metadata": {
    "Sig": "<base64 ed25519 signature>",
    "Pub": "<jwt>",
    "TmV": "2"
  }
}
```

## Path Parameters

`namespace`: e.g. `_` <br/>
`conversationId`: The Conversation Id

## Parameters

See [Message Signing](../README.md#message-signing)

## Query Parameters

`fromAccountId`: Your AccountId <br/>
`sourceMsgId`: Random UUID v4, same as the payload `mid`

---

_Example Response_

Status 201

```json
{
  "conversationId": "GBD2ExampleConversationId00001",
  "msgId": "07bzExampleMessageId02",
  "createdAt": "2026-10-14T18:08:25.783Z",
  "isReportable": false
}
```
