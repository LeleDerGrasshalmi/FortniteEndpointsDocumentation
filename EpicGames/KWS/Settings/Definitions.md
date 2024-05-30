## KWS - Setting Definitions

URL: https://api.kws.ol.epicgames.com/v1/epic-settings/public/users/:accountId/values \
Method: GET \
Auth Required: Yes (`epic-settings:public:games:{game} READ`)

## Path Parameters

`accountId`: Your AccountId

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
        "preferredValue": false,
        "preferredValueUpdatedAt": 1716557959865,
        "preferredValueFromOrgLevel": false,
        "effectiveValue": false,
        "effectiveSource": "preference",
        "isOrgLevel": false,
        "definition": {
          "orgId": "cc5b83aa-cb5c-4b4b-a800-a7dd64edacc0",
          "productId": "6fdb114c-3fbc-4ced-bc5b-55bcdba5c8f6",
          "namespace": "stats",
          "settingName": "show-in-leaderboard",
          "valueType": "boolean",
          "allowProductOverrides": "ageBrackets",
          "inheritFromOrg": true,
          "translations": {
            "en": {
              "label": "Show on career leaderboard",
              "userNotice": "Show on career leaderboard",
              "parentNotice": "Show on career leaderboard"
            }
          },
          "options": [],
          "restrictiveOrder": "falseRestrictive",
          "userHidden": false,
          "required": false,
          "dataStorage": "raw",
          "ageBracket": {
            "consentTypeRequired": "none",
            "consentType": "none",
            "applyConsentToEnforcedUsersOnly": false,
            "defaultValue": true,
            "defaultPreference": true,
            "enforcedLimit": true
          }
        }
      }
    ]
  },
  "meta": {
    "requestId": "85d79fc0-1ea6-11ef-93cc-1d39db92cdb2",
    "timestamp": "2024-05-30T17:03:23.068Z"
  }
}
```
