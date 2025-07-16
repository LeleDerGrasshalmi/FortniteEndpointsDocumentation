## FN EOS Quests Service: Quests

URL: https://fngw-svc-ds-livefn.ol.epicgames.com/api/quest/v3/:deploymentId/progress/account/:accountId \
Method: GET \
Auth Required: Yes (`QuestService Client Feature`)

## Path Parameters

`deploymentId`: The Deployment Id from env configuration, for `live-fn` it is `62a9473a2dca46b29ccf17577fcf42d7` <br/>
`accountId`: Your Account Id

---

_Example Response (shortened)_
```json
{
   "questProgress": {
      "quests": [
         {
            "templateId": "Quest:sparksquest_s09_prestige_ms_02b",
            "productTags": [],
            "state": "Claimed",
            "objectives": [
               {
                  "statName": "sparksquest_s09_prestige_ms_02b_obj0",
                  "quantity": 2,
                  "stage": -1
               }
            ],
            "challengeBundleId": "d838dd81-52a3-44b7-90db-6e58ebe03c09",
            "itemId": "72f26f31-9526-4663-ac1b-1688d05b9cff"
         },
         {
            "templateId": "Quest:quest_s36_ranked_bonusgoal_09",
            "productTags": [],
            "state": "Active",
            "objectives": [
               {
                  "statName": "quest_s36_ranked_bonusgoal_09_obj0",
                  "quantity": 0,
                  "stage": -1
               }
            ],
            "challengeBundleId": "55e850ec-8c4c-4e39-b42f-dbaf181fed65",
            "itemId": "2eae671f-09c1-4c02-845c-7dfacf9ddb46"
         }
      ],
      "challengeBundles": [
         {
            "itemId": "96468f57-2abb-4b7a-8177-2e797cd5be67",
            "templateId": "ChallengeBundle:questbundle_sparks_s08_prestige_ag_pc_01",
            "challengeScheduleId": "9dc3ffa8-bc66-4203-a1ad-0b0e4020f97a",
            "attributes": {
               "num_granted_bundle_quests": 3,
               "num_quests_completed": 3,
               "grantedquestinstanceids": [
                  "2efc27cb-ec13-4479-b607-4cd913e585c9",
                  "f6d160cb-a62a-44d3-a096-06403db63e7e",
                  "b0319cb9-805a-4e65-a31c-f49b34cf7156"
               ],
               "num_progress_quests_completed": 3
            }
         },
         {
            "itemId": "0c40bc33-5326-43e5-b63e-6903d636bd1d",
            "templateId": "ChallengeBundle:questbundle_sparks_s08_kickstart_prestigeunlock",
            "challengeScheduleId": "a5f05261-40dc-4c33-93c7-af7a7e2607e8",
            "attributes": {
               "num_granted_bundle_quests": 1,
               "num_quests_completed": 1,
               "grantedquestinstanceids": [
                  "7c27afcf-9340-45d2-a3b1-d3ee7603045d"
               ],
               "num_progress_quests_completed": 1
            }
         }
      ],
      "challengeBundleSchedules": [
         {
            "itemId": "a5f05261-40dc-4c33-93c7-af7a7e2607e8",
            "templateId": "ChallengeBundleSchedule:sparksseason08_schedule_kickstart",
            "attributes": {
               "unlock_epoch": "2025-04-08T08:00:00.000Z",
               "granted_bundles": [
                  "31231263-dfdb-429f-ad35-f4d3e6b70c58",
                  "0c40bc33-5326-43e5-b63e-6903d636bd1d"
               ]
            }
         },
         {
            "itemId": "c5055cce-86fe-420c-ad9c-7716f94ffd9b",
            "templateId": "ChallengeBundleSchedule:sparksseason08_schedule_milestones",
            "attributes": {
               "unlock_epoch": "2025-04-08T08:00:00.000Z",
               "granted_bundles": [
                  "0bb63d11-89a7-46cf-9c50-20505354b62f"
               ]
            }
         }
      ],
      "trackedQuests": [
         "Quest:quest_forbiddenfruit_kickstart_01_q05"
      ]
   },
   "tokens": [],
   "accountXp": {
      "dynamicXp": {
         "timespan": -1,
         "bucketXp": 0,
         "bankXp": 0,
         "bankXpMult": 1,
         "boosterBucketXp": 0,
         "boosterXpMult": 1,
         "weeklyExcessXpMult": 1,
         "currentWeekXp": 0,
         "currentWeek": 6
      },
      "playtimeXp": {
         "currentWeek": 6,
         "currentWeekXp": 0
      },
      "restedXp": 459235,
      "seasonXp": 59050,
      "seasonLevel": 20,
      "seasonNumber": 36,
      "seasonBegin": "2025-06-01T13:00:00Z",
      "timeDilation": 0
   }
}
```