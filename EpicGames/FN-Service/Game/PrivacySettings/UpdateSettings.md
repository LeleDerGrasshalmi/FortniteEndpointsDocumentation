## FN Service - Update Privacy Settings

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/game/v2/privacy/account/:accountId \
Method: POST \
Auth Required: Yes (`fortnite:profile:{accountId}:commands ALL`)

```js
{
  "optOutOfPublicLeaderboards": true,
  "optOutOfFriendsLeaderboards": false, // obsolete
  "accountId": "94b1569506b04f9f8557af611e8c5e47"
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`optOutOfPublicLeaderboards`: If Stats are public or not <br/>
`optOutOfFriendsLeaderboards`: Obsolete Setting, used handle if friends could fetch your stats (if opted out of public) <br/>
`accountId`: (optional), if specified needs to be your Account Id

---

_Example Response_

```json
{
  "accountId": "94b1569506b04f9f8557af611e8c5e47",
  "optOutOfPublicLeaderboards": false
}
```
