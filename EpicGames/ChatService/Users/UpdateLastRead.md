## Chat Service - Users: Update Last Read

Marks a conversation as read up to a message.

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/users/:accountId/conversations/:conversationId \
Method: PATCH \
Auth Required: Yes (Account Auth)

```json
{
  "msgId": "07c0ExampleMessageId11"
}
```

## Path Parameters

`namespace`: e.g. `_` <br/>
`accountId`: Your AccountId <br/>
`conversationId`: The Conversation Id

## Parameters

`msgId`: The last read Message Id

---

_Example Response_

```json
{}
```
