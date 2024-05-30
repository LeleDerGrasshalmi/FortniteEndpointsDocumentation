## KWS - Update Settings

URL: https://api.kws.ol.epicgames.com/v1/epic-settings/public/users/:accountId/values \
Method: PATCH \
Auth Required: Yes (`epic-settings:public:games:{game} UPDATE`)

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
        "namespace": "stats",
        "settingName": "show-in-leaderboard",
        "effectiveValue": true,
        "effectiveSource": "preference"
      }
    ]
  },
  "meta": {
    "requestId": "48a54900-1eaa-11ef-b3fd-b19a317b502f",
    "timestamp": "2024-05-30T17:30:18.384Z"
  }
}
```
