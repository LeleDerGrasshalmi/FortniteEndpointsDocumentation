## Chat Service - Messages: Send Direct Message

Creates the DM conversation if there is none yet.

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/dm/:accountId/:friendId \
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
`accountId`: Your AccountId <br/>
`friendId`: The receiver AccountId

## Parameters

See [Message Signing](../README.md#message-signing), `rid` is omitted when there is no conversation yet

## Query Parameters

`sourceMsgId`: Random UUID v4, same as the payload `mid`

---

_Example Response_

Status 201

```json
{
  "conversationId": "GBD2ExampleConversationId00001",
  "msgId": "07bzExampleMessageId01",
  "createdAt": "2026-10-14T18:08:25.369Z",
  "isReportable": false
}
```
