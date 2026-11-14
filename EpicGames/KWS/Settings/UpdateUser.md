## KWS - Update User

Sets the time zone of the account. The Epic Games Launcher sends it at every sign-in.

URL: https://api.kws.ol.epicgames.com/v1/epic-settings/public/users/:accountId \
Method: PATCH \
Auth Required: Yes (Account Auth)

```json
{
  "clientTimeZone": "America/New_York"
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`clientTimeZone`: IANA time zone name

---

_Example Response_

```json
{
  "response": {
    "userId": "94b1569506b04f9f8557af611e8c5e47",
    "clientTimeZone": "America/New_York"
  },
  "meta": {
    "requestId": "8283e81f-6175-4706-aa82-d6c93ee79a7c",
    "timestamp": "2026-11-14T03:01:00.268Z"
  }
}
```
