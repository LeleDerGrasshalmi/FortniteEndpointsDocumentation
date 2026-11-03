## Chat Service - Conversations: Update Title

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/conversations/:conversationId \
Method: PATCH \
Auth Required: Yes (Account Auth)

```json
{
  "title": "Docs Test Renamed"
}
```

## Path Parameters

`namespace`: e.g. `_` <br/>
`conversationId`: The Conversation Id

## Parameters

`title`: The new group title

## Query Parameters

`requestingAccountId`: Your AccountId

---

_Example Response_: Status 200 with an empty body

The change is added to the history as a `social.chat.v1.TITLE_CHANGE` system entry, see [Conversation Messages](../Messages/Messages.md)
