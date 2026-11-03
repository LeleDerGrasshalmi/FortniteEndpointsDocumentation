## Chat Service - Users: Summary

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/users/:accountId/summary \
Method: GET \
Auth Required: Yes (Account Auth)

## Path Parameters

`namespace`: e.g. `_` <br/>
`accountId`: Your AccountId

---

_Example Response_

```json
{
  "conversationCount": 1,
  "unreadMessages": 1,
  "unreadPendingInvites": 0,
  "hasMoreUnreadMessages": false,
  "hasMoreUnreadPendingInvites": false
}
```
