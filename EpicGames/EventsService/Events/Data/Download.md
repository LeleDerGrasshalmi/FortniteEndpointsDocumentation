## Events Service - Events List (Download)

URL: https://events-public-service-live.ol.epicgames.com/api/v1/events/:gameId/download/:accountId \
Method: GET \
Auth Required: Yes (`{gameId}:profile:{accountId}:commands READ`)

## Path Parameters

`gameId`: Fortnite <br/>
`accountId`: Your Account Id

## Query Parameters

`region`: required, e.g. EU <br/>
`platform`: required, e.g. Windows <br/>
`teamAccountIds`: required, Account Ids seperated by a comma `,`

---

_Example Response (shortened)_

```json
{
  "events": [
    {
      "gameId": "Fortnite",
      "eventId": "epicgames_S25_DuosFillQuickCup_EU",
      "regions": ["EU"],
      "regionMappings": {},
      "platforms": ["PS4", "XboxOne", "XSX", "Android", "PS5", "Windows"],
      "platformMappings": {},
      "displayDataId": "s25_fill_duosbr",
      "eventGroup": "Season25DuosFillQuickCup",
      "announcementTime": "2023-06-09T15:00:00.000Z",
      "appId": null,
      "environment": null,
      "link": {
        "type": "br:tournament",
        "code": "tournament_epicgames_s25_duosfillquickcup_eu",
        "version": 1
      },
      "metadata": {
        "TeamLockType": "Window",
        "minimumAccountLevel": 15,
        "TrackedStats": ["MMO_RadioTower", "MMO_LootIsland"],
        "DisqualifyType": "Event",
        "RegionLockType": "None",
        "AccountLockType": "Window"
      },
      "eventWindows": [
        {
          "eventWindowId": "S25_DuosFillQuickCup_Event1_EU",
          "eventTemplateId": "EventTemplate_S25_DuosFillQuickCup_EU",
          "countdownBeginTime": "2023-06-15T15:00:00.000Z",
          "beginTime": "2023-06-15T17:00:00.000Z",
          "endTime": "2023-06-15T20:00:00.000Z",
          "blackoutPeriods": [],
          "round": 0,
          "payoutDelay": 32,
          "isTBD": false,
          "canLiveSpectate": false,
          "scoreLocations": [
            {
              "leaderboardDefId": "S25_BRDuosQuickFill_DefaultLeaderboardDef",
              "windowEndCondition": null,
              "isMainWindowLeaderboard": true
            }
          ],
          "visibility": "public",
          "requireAllTokens": [],
          "requireAnyTokens": [],
          "requireNoneTokensCaller": ["Season25DuosFillQuickCup_NAC"],
          "requireAllTokensCaller": [],
          "requireAnyTokensCaller": [],
          "additionalRequirements": [
            "mfa",
            "eula:s25_fill_rules",
            "currentRanking:ranked-br:3"
          ],
          "teammateEligibility": "all",
          "regionMappings": null,
          "metadata": {
            "ServerReplays": true,
            "RoundType": "Qualifiers",
            "liveSpectateAccessToken": "WeeklyTournamentSpectator"
          }
        }
      ],
      "beginTime": "2023-06-15T17:00:00.000Z",
      "endTime": "2023-10-18T20:00:00.000Z"
    }
  ],
  "templates": [
    {
      "gameId": "Fortnite",
      "eventTemplateId": "EventTemplate_S25_DuosFillQuickCup_EU",
      "playlistId": "Playlist_ShowdownTournament_FillOnly_Duos",
      "matchCap": 10,
      "liveSessionAttributes": [],
      "scoringRules": [],
      "tiebreakerFormula": {
        "basePointsBits": 11,
        "components": [
          {
            "trackedStat": "VICTORY_ROYALE_STAT",
            "bits": 4,
            "multiplier": null,
            "aggregation": "sum"
          },
          {
            "trackedStat": "TEAM_ELIMS_STAT_INDEX",
            "bits": 12,
            "multiplier": 100.0,
            "aggregation": "avg"
          }
        ]
      },
      "payoutTable": [
        {
          "scoreId": null,
          "scoringType": "value",
          "ranks": [
            {
              "threshold": 0.0,
              "payouts": [
                {
                  "rewardType": "token",
                  "rewardMode": "rolling",
                  "value": "Season25DuosFillQuickCup_EU",
                  "quantity": 1
                }
              ]
            }
          ]
        }
      ],
      "onlyScoreTopN": null,
      "clampsToZero": false
    }
  ],
  "leaderboardDefs": [
    {
      "gameId": "Fortnite",
      "leaderboardDefId": "S25_BRDuosQuickFill_DefaultLeaderboardDef",
      "leaderboardStorageId": "Fortnite_GLOBAL",
      "leaderboardInstanceGroupingKeyFormat": "${eventId}",
      "leaderboardInstanceIdFormat": "${windowId}",
      "maxSessionHistorySize": 10,
      "onlyScoreTopN": null,
      "useIndividualScores": false,
      "tiebreakerFormula": {
        "basePointsBits": 11,
        "components": [
          {
            "trackedStat": "VICTORY_ROYALE_STAT",
            "bits": 4,
            "multiplier": null,
            "aggregation": "sum"
          }
        ]
      },
      "scoringRuleSetId": "S26_ScoringRules_ConsoleChampionsCup",
      "clampsToZero": true,
      "payoutsConfig": null,
      "bestNTeams": null,
      "hidePlayerScores": false,
      "percentileAccuracy": null,
      "requiredPlayerListings": []
    }
  ],
  "scoringRuleSets": {
    "S26_ScoringRules_ConsoleChampionsCup": [
      {
        "trackedStat": "PLACEMENT_STAT_INDEX",
        "matchRule": "lte",
        "rewardTiers": [
          {
            "keyValue": 1,
            "pointsEarned": 9,
            "multiplicative": false
          }
        ]
      },
      {
        "trackedStat": "TEAM_ELIMS_STAT_INDEX",
        "matchRule": "gte",
        "rewardTiers": [
          {
            "keyValue": 1,
            "pointsEarned": 4,
            "multiplicative": true
          }
        ]
      }
    ]
  },
  "payoutTables": {},
  "resolvedWindowLocations": {
    "Fortnite:epicgames_S25_DuosFillQuickCup_EU:S25_DuosFillQuickCup_Event1_EU": [
      "Fortnite:epicgames_S25_DuosFillQuickCup_EU:S25_DuosFillQuickCup_Event1_EU"
    ]
  }
}
```
