## Chat Service - Messages: Reportable Messages

Messages around a reported message. Only `social.chat.v1.NEW_MESSAGE` entries, oldest first, system entries are left out.

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/conversations/:conversationId/reportable-messages \
Method: GET \
Auth Required: Yes (Account Auth)

## Path Parameters

`namespace`: e.g. `_` <br/>
`conversationId`: The Conversation Id

## Query Parameters

`requestingAccountId`: Your AccountId <br/>
`reportedMessageId`: The reported Message Id <br/>
`contextWindowSize`: Optional, e.g. `25`

---

_Example Response (Reportable Conversation)_

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
      "msgId": "07c0ExampleMessageId25",
      "senderId": "94b1569506b04f9f8557af611e8c5e47",
      "createdAt": "2026-10-14T22:31:32.281Z",
      "isReportable": true,
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
      "msgId": "07c0ExampleMessageId26",
      "senderId": "5e2d8c1b9a7f4e3d8c6b2a1f0e9d7c3b",
      "createdAt": "2026-10-14T22:31:35.66Z",
      "isReportable": true,
      "message": {
        "body": "<base64 payload>"
      }
    }
  ],
  "hasNextPage": false
}
```

_Example Response (Conversation with `isReportable: false`)_

```json
{
  "page": [],
  "hasNextPage": false
}
```
