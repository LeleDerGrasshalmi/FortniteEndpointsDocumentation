## KWS - Update Settings

URL: https://api.kws.ol.epicgames.com/v1/epic-settings/public/users/:accountId/values \
Method: GET \
Auth Required: Yes (`epic-settings:public:games:{game} READ`)

```json
{
  "game": "fn",
  "parentPIN": "",
  "settings": [
    {
      "namespace": "stats",
      "settingName": "show-in-leaderboard",
      "preferredValue": true
    }
  ],
  "initialSync": false
}
```

## Path Parameters

`accountId`: Your AccountId

## Parameters

`game`: Same as your `game` query <br/>
`parentPIN`: The PIN if Parental Controls are enabled and if the pin required (e.g. changing `stats`.`show-in-leaderboard` doesnt require it) <br/>
`settings`: New Setting Values <br/>
`settings.namespace`: The namespace of the setting, e.g. `stats` <br/>
`settings.settingName`: The name of the setting, e.g. `show-in-leaderboard` <br/>
`settings.preferredValue`: The new setting value, check the setting definition for the expected type <br/>
`initialSync`: Whether you are first creating the Settings/KWS

## Query Parameters

`game`: For Fortnite it's `fn`

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
