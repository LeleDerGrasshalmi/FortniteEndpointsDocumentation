## Friends Service - Friendship Info

URL: https://friends-public-service-prod.ol.epicgames.com/friends/api/v1/:accountId/friends/:friendId <br/>
Method: GET <br/>
Auth Required: Yes (`friends:{accountId} READ`)

## Path Parameters

`accountId`: Your Account Id <br/>
`friendId`: Friend Account Id

---

*Example Response (success)*

```json
{
  "accountId": "0204ef14e09a48f7846cc8127f860507",
  "groups": [],
  "mutual": 92,
  "alias": "",
  "note": "",
  "favorite": false,
  "created": "2022-11-19T23:01:12.537Z"
}
```

*Example Response (friend not found)*

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
