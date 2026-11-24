## Chat Service - Users: Summary

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/users/:accountId/summary <br/>
Method: GET <br/>
Auth Required: Yes (Account Auth)

## Path Parameters

`namespace`: e.g. `_` <br/>
`accountId`: Your AccountId

---

*Example Response*

```json
{
  "conversationCount": 1,
  "unreadMessages": 1,
  "unreadPendingInvites": 0,
  "hasMoreUnreadMessages": false,
  "hasMoreUnreadPendingInvites": false
}
```
