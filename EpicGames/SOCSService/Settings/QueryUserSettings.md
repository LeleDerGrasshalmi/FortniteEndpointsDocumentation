## SOCS Service - Settings: Query User Settings

URL: https://api.epicgames.dev/epic/socs/v1/users/:accountId/settings/query \
Method: POST \
Auth Required: Yes (Account Auth)

```json
{
  "scopeMatchFilters": {
    "v1Platform": ["Windows"]
  }
}
```

## Path Parameters

`accountId`: Your AccountId

## Parameters

`scopeMatchFilters`: Filters for scoped settings, e.g. `v1Platform`

---

_Example Response_

```json
{
  "settings": [
    {
      "id": "v1AccessibilityAllowVoiceDictation",
      "userOverrides": [],
      "default": "false"
    },
    {
      "id": "v1AccessibilityReadMessagesAloud",
      "userOverrides": [],
      "default": "false"
    },
    {
      "id": "v1AgeVerificationChatRestrictionNotificationSeen",
      "userOverrides": [],
      "default": "false"
    },
    {
      "id": "v1EpicPartiesProfileMoveHasSeenDisclosure",
      "userOverrides": [],
      "default": "true"
    },
    {
      "id": "v1GlobalNicknamesHasSeenDisclosure",
      "userOverrides": [
        {
          "scopes": {},
          "value": "true"
        }
      ],
      "default": "false"
    },
    {
      "id": "v1VoiceChatMode",
      "userOverrides": [],
      "default": "openMic"
    },
    {
      "id": "v1VoiceChatReportingDisclosureAcceptanceStatus",
      "userOverrides": [
        {
          "scopes": {},
          "value": "seen-accepted"
        }
      ],
      "default": "never-shown"
    },
    {
      "id": "v1VoiceInputDevice",
      "userOverrides": [],
      "default": ""
    },
    {
      "id": "v1VoiceInputVolume",
      "userOverrides": [],
      "default": "50"
    },
    {
      "id": "v1VoiceOutputDevice",
      "userOverrides": [],
      "default": ""
    },
    {
      "id": "v1VoiceOutputVolume",
      "userOverrides": [],
      "default": "50"
    },
    {
      "id": "v1VoicePushToTalkKeybinding",
      "userOverrides": [],
      "default": ""
    }
  ]
}
```
