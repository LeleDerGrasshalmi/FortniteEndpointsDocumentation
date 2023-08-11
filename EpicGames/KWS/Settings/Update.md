## KWS - Update Settings

URL: https://api.kws.ol.epicgames.com/v1/epic-settings/public/users/:accountId/values \
Method: PATCH \
Auth Required: Yes

## Path Parameters

`accountId`: Your AccountId

## Query Parameters

`game`: For Fortnite it's 'fn'

---

_Example Response (shortened)_

```json
{
  "response": {
    "settings": [
      {
        "namespace": "profile",
        "settingName": "allow-non-squad-users-to-see-my-username",
        "effectiveValue": true,
        "effectiveSource": "preference"
      }
    ]
  },
  "meta": {
    "requestId": "cce500d0-a0dd-11ed-9f30-8bbd96c54a31",
    "timestamp": "2023-01-30T20:36:40.413Z"
  }
}
```
