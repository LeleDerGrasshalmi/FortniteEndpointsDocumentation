## FN Service - Calendar

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/calendar/v1/timeline \
Method: GET \
Auth Required: Yes (`fortnite:calendar READ`)

---

_Example Response (shortened)_

```json
{
  "channels": {
    "standalone-store": {
      "states": [
        {
          "validFrom": "2023-05-18T22:05:32.216Z",
          "activeEvents": [],
          "state": {
            "activePurchaseLimitingEventIds": [],
            "storefront": {},
            "rmtPromotionConfig": [],
            "storeEnd": "0001-01-01T00:00:00.000Z"
          }
        }
      ],
      "cacheExpire": "2023-05-19T00:05:32.216Z"
    },
    "client-matchmaking": {
      "states": [
        {
          "validFrom": "2023-05-18T22:05:32.216Z",
          "activeEvents": [],
          "state": {
            "region": {
              "OCE": {
                "eventFlagsForcedOff": ["Playlist_DefaultDuo"]
              },
              "CN": {
                "eventFlagsForcedOff": [
                  "Playlist_DefaultDuo",
                  "Playlist_Bots_DefaultDuo",
                  "Playlist_Deimos_DuoCN"
                ]
              },
              "REGIONID": {
                "eventFlagsForcedOff": ["Playlist_Deimos_Duo_WinterCN"]
              },
              "ASIA": {
                "eventFlagsForcedOff": ["Playlist_DefaultDuo"]
              }
            }
          }
        }
      ],
      "cacheExpire": "2023-05-19T00:05:32.216Z"
    },
    "tk": {
      "states": [
        {
          "validFrom": "2023-05-18T22:05:32.216Z",
          "activeEvents": [],
          "state": {
            "k": [
              "B3D2793477E5D467475BE403774360E5:HNj5inGk1/2h9f0r4+SGPPY9t69eOwS6w0XGxpTVOTM="
            ]
          }
        }
      ],
      "cacheExpire": "2023-05-19T00:05:32.216Z"
    },
    "featured-islands": {
      "states": [
        {
          "validFrom": "2023-05-18T22:05:32.216Z",
          "activeEvents": [],
          "state": {
            "islandCodes": [],
            "playlistCuratedContent": {},
            "playlistCuratedHub": {
              "Playlist_PlaygroundV2": "4707-3216-0421",
              "Playlist_Creative_PlayOnly": "4707-3216-0421"
            },
            "islandTemplates": []
          }
        }
      ],
      "cacheExpire": "2023-05-19T00:05:32.216Z"
    },
    "community-votes": {
      "states": [
        {
          "validFrom": "2023-05-18T22:05:32.216Z",
          "activeEvents": [],
          "state": {
            "electionId": "",
            "candidates": [],
            "electionEnds": "9999-12-31T23:59:59.999Z",
            "numWinners": 1
          }
        }
      ],
      "cacheExpire": "2023-05-19T00:05:32.216Z"
    },
    "client-events": {
      "states": [
        {
          "validFrom": "2023-05-18T22:05:32.216Z",
          "activeEvents": [
            {
              "eventType": "EventFlag.Event_DarkIce",
              "activeUntil": "2023-08-08T13:00:00.000Z",
              "activeSince": "2023-05-18T13:00:00.000Z"
            }
          ],
          "state": {
            "activeStorefronts": [],
            "eventNamedWeights": {},
            "activeEvents": [
              {
                "instanceId": "5fjc9793egmn7df10ca3m36nug[2]0",
                "devName": "Event_DarkIce",
                "eventName": "CalendarEvent_DarkIce",
                "eventStart": "2023-05-18T13:00:00Z",
                "eventEnd": "2023-08-08T13:00:00Z",
                "eventType": "EventFlag.Event_DarkIce"
              }
            ],
            "seasonNumber": 24,
            "seasonTemplateId": "AthenaSeason:athenaseason24",
            "matchXpBonusPoints": 0,
            "eventPunchCardTemplateId": "",
            "seasonBegin": "2023-03-09T13:00:00Z",
            "seasonEnd": "2023-06-18T12:00:00Z",
            "seasonDisplayedEnd": "2023-06-04T04:00:00Z",
            "weeklyStoreEnd": "2023-05-19T00:00:00Z",
            "stwEventStoreEnd": "2023-06-22T00:00:00.000Z",
            "stwWeeklyStoreEnd": "2023-05-25T00:00:00.000Z",
            "sectionStoreEnds": {
              "Daily": "2023-05-19T00:00:00Z",
              "Featured": "2023-05-19T00:00:00Z"
            },
            "rmtPromotion": "",
            "dailyStoreEnd": "2023-05-19T00:00:00Z"
          }
        }
      ],
      "cacheExpire": "2023-05-19T00:05:32.216Z"
    }
  },
  "cacheIntervalMins": 15,
  "currentTime": "2023-05-18T22:29:42.758Z"
}
```
