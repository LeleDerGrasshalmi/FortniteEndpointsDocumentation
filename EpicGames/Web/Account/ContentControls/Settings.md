## Account Web - Content Controls: Get

URL: https://www.epicgames.com/account/v2/content-controls/get \
Method: GET \
Auth Required: Yes

---

_Example Response_

```json
{
  "success": true,
  "data": {
    "controlsEnabled": false,
    "pinGatedPurchasingEnabled": false,
    "principalId": "",
    "metaData": {
      "pinGatedPurchasingEnabled": false,
      "ageGateSystem": "ESRB",
      "ageGateData": {
        "name": "Everyone",
        "age": 3
      },
      "level": 0
    },
    "supervisedSettings": {
      "text": {
        "namespace": "chat",
        "settingName": "text"
      },
      "require-pin-to-add-friend": {
        "namespace": "profile",
        "settingName": "require-pin-to-add-friend"
      },
      "filter-out-mature-language": {
        "namespace": "chat",
        "settingName": "filter-out-mature-language"
      },
      "voice": {
        "namespace": "chat",
        "settingName": "voice"
      },
      "playtime-reporting-frequency": {
        "namespace": "profile",
        "settingName": "playtime-reporting-frequency"
      }
    },
    "supervisedSettingsDefinition": {
      "text": {
        "options": [
          {
            "value": "nobody",
            "translations": {
              "label": "Nobody",
              "parentNotice": "Epic text chat is disabled for your child."
            }
          },
          {
            "value": "friends",
            "translations": {
              "label": "Friends Only",
              "parentNotice": "Your child can text chat only with players in their Epic friends list and platform friends list."
            }
          },
          {
            "value": "friends-and-teammates",
            "translations": {
              "label": "Friends & Teammates",
              "parentNotice": "Your child can text chat with players in their Epic friends list and platform friends list, and those on their team."
            }
          },
          {
            "value": "everybody",
            "translations": {
              "label": "Everybody",
              "parentNotice": "Your child can text chat with any player."
            }
          }
        ],
        "valueType": "option",
        "restrictiveOrder": "firstRestrictive",
        "translations": {
          "label": "Voice chat",
          "parentNotice": "Who can your child message with using Epic text chat?"
        }
      },
      "require-pin-to-add-friend": {
        "options": [],
        "valueType": "boolean",
        "restrictiveOrder": "falsePermissive",
        "translations": {
          "label": "Require PIN to add Epic friends",
          "parentNotice": "<b>On:</b> Each time your child tries to send or accept an Epic Games friend request, you will need to enter your PIN. If a game or service doesn't yet support this setting, friend requests won't be permitted. This setting doesn’t affect friends systems on gaming platforms such as Playstation, Steam, XBox, and Switch."
        }
      },
      "filter-out-mature-language": {
        "options": [],
        "valueType": "boolean",
        "restrictiveOrder": "falsePermissive",
        "translations": {
          "label": "Filter out mature language in Epic text chat",
          "parentNotice": "<b>On:</b> Mature language in text chat will be filtered and replaced with heart symbols."
        }
      },
      "voice": {
        "options": [
          {
            "value": "nobody",
            "translations": {
              "label": "Nobody",
              "parentNotice": "Epic voice chat is disabled for your child."
            }
          },
          {
            "value": "friends",
            "translations": {
              "label": "Friends Only",
              "parentNotice": "Your child can voice chat only with players in their Epic friends list and platform friends list."
            }
          },
          {
            "value": "friends-and-teammates",
            "translations": {
              "label": "Friends & Teammates",
              "parentNotice": "Your child can voice chat with players in their Epic friends list and platform friends list, and those on their team."
            }
          },
          {
            "value": "everybody",
            "translations": {
              "label": "Everybody",
              "parentNotice": "Your child can voice chat with any player."
            }
          }
        ],
        "valueType": "option",
        "restrictiveOrder": "firstRestrictive",
        "translations": {
          "label": "Voice chat",
          "parentNotice": "Who can your child speak with using Epic voice chat?"
        }
      },
      "playtime-reporting-frequency": {
        "options": [
          {
            "value": "weekly",
            "translations": {
              "label": "Weekly",
              "parentNotice": "<b>On:</b> We'll send a weekly playtime report to the parent or guardian associated with this account. If there isn't a parent or guardian email address, we'll send the playtime report to this account’s email address."
            }
          },
          {
            "value": "never",
            "translations": {
              "label": "Never",
              "parentNotice": "<b>Off:</b> You won't receive weekly playtime tracking reports."
            }
          }
        ],
        "valueType": "option",
        "restrictiveOrder": "firstRestrictive",
        "translations": {
          "label": "Receive weekly playtime tracking reports",
          "parentNotice": "Receive weekly playtime tracking reports"
        }
      }
    }
  }
}
```
