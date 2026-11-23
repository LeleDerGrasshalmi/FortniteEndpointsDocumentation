## Friends Service - Decline Incoming / Cancel Outgoing / Remove Friend

URL: https://friends-public-service-prod.ol.epicgames.com/friends/api/v1/:accountId/friends/:friendId <br/>
Method: DELETE <br/>
Auth Required: Yes (`friends:{accountId} DELETE`)

## Path Parameters

`accountId`: Your Account Id <br/>
`friendId`: Friend Account Id

---

*Example Response (cancel outgoing, delete friend)*: Status 204

*Example Response (not a friend)*

```json
{
  "errorCode": "errors.com.epicgames.friends.friendship_not_found",
  "errorMessage": "Friendship between 94b1569506b04f9f8557af611e8c5e47 and 3a041fc98f2f4627912935b451e947fc does not exist",
  "messageVars": [
    "94b1569506b04f9f8557af611e8c5e47",
    "3a041fc98f2f4627912935b451e947fc"
  ],
  "numericErrorCode": 14004,
  "originatingService": "friends",
  "intent": "prod"
}
```
