## FN Service - Update Privacy Settings

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/game/v2/privacy/account/:accountId <br/>
Method: POST <br/>
Auth Required: Yes (`fortnite:profile:{accountId}:commands ALL`)

```json
{
  "optOutOfPublicLeaderboards": true,
  "accountId": "94b1569506b04f9f8557af611e8c5e47"
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`optOutOfPublicLeaderboards`: If Stats are public or not <br/>
`accountId`: (optional), if specified needs to be your Account Id

---

*Example Response*

```json
{
  "accountId": "94b1569506b04f9f8557af611e8c5e47",
  "optOutOfPublicLeaderboards": false
}
```
