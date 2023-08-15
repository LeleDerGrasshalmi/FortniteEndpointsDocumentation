## Wex Service - Calendar Timeline

URL: https://wex-public-service-live-prod.ol.epicgames.com/wex/api/calendar/v1/timeline \
Method: GET \
Auth Required: Yes (`wexp:calendar READ`)

---

_Example Response (shortened)_

```json
{
  "channels": {
    "news": {
      "states": [
        {
          "validFrom": "2022-11-10T17:35:10.400Z",
          "activeEvents": [],
          "state": {}
        }
      ],
      "cacheExpire": "2022-11-10T19:35:10.400Z"
    },
    "limited-time-mode": {
      "states": [
        {
          "validFrom": "2022-11-10T17:35:10.400Z",
          "activeEvents": [],
          "state": {
            "activeLTMs": [
              {
                "LTM_Event_ID": "Week2_LTM",
                "LTM_ID": "Endless_01",
                "PlayMode": {
                  "Mode": "DeepDungeons",
                  "Rules": [
                    {
                      "Rule": "AgilityHeroBonus",
                      "RuleDataValue": 0
                    },
                    {
                      "Rule": "StrongSpecial",
                      "RuleDataValue": 0
                    }
                  ],
                  "Zones": [
                    {
                      "ZoneId": "Zone.LeafyTreeland.Map5",
                      "Difficulty": "Easy",
                      "completionLoot": "LTG.LTM.Endless.Completion.VeryLow"
                    },
                    {
                      "ZoneId": "Zone.OasisOfLife.Map3",
                      "Difficulty": "Easy",
                      "firstCompletionLoot": "LTG.LTM.Battlepass5_Week2.FirstCompletion",
                      "completionLoot": "LTG.LTM.Battlepass5_Week2.Endless.Low.Gear"
                    }
                  ],
                  "ModeDataValue": 0,
                  "ImageIndex": 113
                },
                "modeNamedWeight": "Modes_TimeAttack",
                "ruleNamedWeights": [
                  "Rules_AgilityHeroBonus",
                  "Rules_StrongSpecial",
                  "Rules_FastCoolDown"
                ],
                "availabilityBegin": "2022-11-09T00:00:00.000Z",
                "availabilityEnd": "2022-11-16T00:00:00.000Z"
              }
            ],
            "eventInstanceId": "$EVENT_INSTANCE_ID"
          }
        }
      ],
      "cacheExpire": "2022-11-10T19:35:10.400Z"
    },
    "marketing": {
      "states": [
        {
          "validFrom": "2022-11-10T17:35:10.400Z",
          "activeEvents": [],
          "state": {
            "affiliateSelectionEndDate": "0001-01-01T00:00:00.000Z"
          }
        }
      ],
      "cacheExpire": "2022-11-10T19:35:10.400Z"
    },
    "rotational-content": {
      "states": [
        {
          "validFrom": "2022-11-10T17:35:10.400Z",
          "activeEvents": [],
          "state": {
            "activeZones": [
              {
                "sortPriority": 800,
                "zoneId": "Zone.Event.GrandArena.Aux.Battleford.Map1",
                "maxRuns": -1,
                "resetCostMtx": 0,
                "flags": ["IsSpecialEvent"],
                "eventId": "Event.GrandArena",
                "dynamicTier": 1,
                "dynamicGoldTier": 1,
                "dynamicWorldLevel": -1,
                "expiresAt": "2026-01-01T00:00:00Z",
                "eventKey": "37m008vr790voua5ie1g0s0pqg[0]0+0"
              }
            ],
            "activeEvents": [
              {
                "sortPriority": 999,
                "eventAsset": "/Game/Campaign/Zones/Events/Evergreen3/EventDef_Evergreen3.EventDef_Evergreen3",
                "eventId": "2020_2",
                "expiresAt": "2022-11-30T00:00:00Z"
              }
            ],
            "preregRewardZones": [],
            "heroStoreEnd": "2022-11-14T00:00:00.000Z",
            "purchasingEventId": "Event.DarkGenerals"
          }
        }
      ],
      "cacheExpire": "2022-11-10T19:35:10.400Z"
    },
    "featured-stores-mcp": {
      "states": [
        {
          "validFrom": "2022-11-10T17:35:10.400Z",
          "activeEvents": [],
          "state": {
            "activePurchaseLimitingEventIds": [],
            "storefront": {}
          }
        }
      ],
      "cacheExpire": "2022-11-10T19:35:10.400Z"
    },
    "weekly-challenge": {
      "states": [
        {
          "validFrom": "2022-11-10T17:35:10.400Z",
          "activeEvents": [],
          "state": {
            "phases": [
              {
                "zoneId": "Zone.Event.WC.Daily.BossDuo.Map1",
                "availabilityBegin": "2022-11-07T00:00:00.000Z",
                "availabilityEnd": "2022-11-14T00:00:00.000Z",
                "minAccountLevel": 1,
                "maxAccountLevel": 2147483647,
                "requirements": {
                  "maxPartySize": 5,
                  "minPartySize": 1,
                  "requirements": [
                    {
                      "count": 1,
                      "heroClass": "Knight",
                      "heroElement": "None"
                    }
                  ],
                  "excludeClasses": [],
                  "excludeElements": []
                }
              }
            ],
            "activePhases": [
              "Weekend",
              "Monday",
              "Tuesday",
              "Wednesday",
              "Thursday",
              "Friday"
            ],
            "eventInstanceId": "70ruue8l0oma4lm9egb3o9koga[0]151",
            "bossZone": {
              "zoneId": "Zone.Event.WC.Weekend.BossSuper.1.EternalDeterrent.Map1",
              "availabilityBegin": "2022-11-07T00:00:00.000Z",
              "availabilityEnd": "2022-11-14T00:00:00.000Z",
              "minAccountLevel": 1,
              "maxAccountLevel": 2147483647,
              "runLimit": 1
            },
            "namedWeights": "EternalDeterrent=1"
          }
        }
      ],
      "cacheExpire": "2022-11-10T19:35:10.400Z"
    },
    "battlepass": {
      "states": [
        {
          "validFrom": "2022-11-10T17:35:10.400Z",
          "activeEvents": [],
          "state": {
            "seasonId": "2020_2",
            "seasonEndDate": "2022-11-30T00:00:00Z"
          }
        }
      ],
      "cacheExpire": "2022-11-10T19:35:10.400Z"
    }
  },
  "cacheIntervalMins": 15,
  "currentTime": "2022-11-10T17:52:47.351Z"
}
```
