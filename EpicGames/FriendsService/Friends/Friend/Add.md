## Friends Service - Accept Incoming / Send Outgoing

URL: https://friends-public-service-prod.ol.epicgames.com/friends/api/v1/:accountId/friends/:friendId <br/>
Method: POST <br/>
Auth Required: Yes (`friends:{accountId} UPDATE`)

```json
{
  "pin": "123456"
}
```

## Path Parameters

`accountId`: Your Account Id <br/>
`friendId`: Friend Account Id

## Parameters

`pin`: The required parental controls pin, that is required when its configured, that friend management needs the pin

---

*Example Response (success)*: Status 204

*Example Response (other account has friend requests disabled)*

```json
{
  "errorCode": "errors.com.epicgames.friends.cannot_friend_due_to_target_settings",
  "errorMessage": "Account 94b1569506b04f9f8557af611e8c5e47 cannot friend 3a041fc98f2f4627912935b451e947fc because of invitee's privacy settings",
  "messageVars": [
    "94b1569506b04f9f8557af611e8c5e47",
    "3a041fc98f2f4627912935b451e947fc"
  ],
  "numericErrorCode": 14120,
  "originatingService": "friends",
  "intent": "prod"
}
```
