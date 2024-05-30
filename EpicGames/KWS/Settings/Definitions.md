## KWS - Setting Definitions

URL: https://api.kws.ol.epicgames.com/v1/epic-settings/public/users/:accountId/values \
Method: GET \
Auth Required: Yes (`epic-settings:public:games:{game} READ`)

```json
{
  "game": "fn",
  "parentPIN": "",
  "settings": [
    {
      "namespace": "profile",
      "settingName": "allow-non-squad-users-to-see-my-username",
      "preferredValue": true
    }
  ],
  "initialSync": true
}
```

## Path Parameters

`accountId`: Your AccountId

## Parameters

`game`: Same as your query 'game' <br/>
`parentPIN`: The PIN if Parental Controls are enabled <br/>
`settings`: New Setting Values <br/>
`initialSync`: Whether you are first creating the Settings/KWS

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
        "preferredValue": true,
        "preferredValueFromOrgLevel": true,
        "effectiveValue": true,
        "effectiveSource": "default",
        "isOrgLevel": true,
        "definition": {
          "orgId": "cc5b83aa-cb5c-4b4b-a800-a7dd64edacc0",
          "productId": "6fdb114c-3fbc-4ced-bc5b-55bcdba5c8f6",
          "namespace": "profile",
          "settingName": "allow-non-squad-users-to-see-my-username",
          "valueType": "boolean",
          "allowProductOverrides": "ageBrackets",
          "inheritFromOrg": true,
          "translations": {
            "en": {
              "label": "Display username to non-squad users",
              "userNotice": "Determines if your username can be shown to non-squad users",
              "parentNotice": "Determines if your child''s username can be shown to non-squad users"
            }
          },
          "options": [],
          "restrictiveOrder": "falseRestrictive",
          "userHidden": false,
          "userReadOnly": false,
          "required": false,
          "ageBracket": {
            "consentTypeRequired": "none",
            "defaultValue": true
          }
        }
      }
    ]
  },
  "meta": {
    "requestId": "3ba7b140-a0af-11ed-8e07-95866a481c07",
    "timestamp": "2023-01-30T15:03:19.892Z"
  }
}
```
