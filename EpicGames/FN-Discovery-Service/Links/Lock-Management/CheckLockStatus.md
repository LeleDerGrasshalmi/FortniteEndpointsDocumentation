## FN - Discovery Service: Check Links Lock Status

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v1/links/lock-status/:accountId/check \
Method: POST \
Auth Required: Yes (`discovery:{accountId}:links:lock-management READ`)

```json
{
  "linkCodes": ["1111-1111-1111"]
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`linkCodes`: The Mnemonics to check

---

_Example Response_

```json
{
  "results": [
    {
      "playerId": "94b1569506b04f9f8557af611e8c5e47",
      "linkCode": "1111-1111-1111",
      "lockStatus": "UNLOCKED",
      "lockStatusReason": "NONE",
      "isVisible": true
    }
  ],
  "hasMore": false
}
```
