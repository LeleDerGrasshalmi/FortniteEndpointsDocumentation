## Party Service - Get Party Info by Account Id

URL: https://party-service-prod.ol.epicgames.com/party/api/v1/Fortnite/user/:accountId \
Method: GET \
Auth Required: Yes (`social:party`)

## Path Parameters

`accountId`: Your AccountId

_Example Response (shortened)_

```json
{
    "current": [
        {
            "id": "47ccf96757ab4ce3a37c83e0a53ba7b9",
			"created_at": "2025-09-24T16:57:04.662Z",
			"updated_at": "2025-09-24T16:57:06.426Z",
			"config": {
				"type": "DEFAULT",
				"joinability": "INVITE_AND_FORMER",
				"discoverability": "INVITED_ONLY",
				"sub_type": "default",
				"max_size": 16,
				"invite_ttl": 14400,
				"join_confirmation": true,
				"intention_ttl": 7200
			},
            "members": [
                {
                    "account_id": "b1c60df4f45a4b51b763eac539326664",
                    "meta": {
                        "Default:AthenaCosmeticLoadout_j": "{\"AthenaCosmeticLoadout\":{\"characterPrimaryAssetId\":\"AthenaCharacter:Character_BoldTouch\",\"characterEKey\":\"\",\"backpackDef\":\"/BRCosmetics/Athena/Items/Cosmetics/Backpacks/Backpack_CamelGram.Backpack_CamelGram\",\"backpackEKey\":\"\",\"pickaxeDef\":\"/BRCosmetics/Athena/Items/Cosmetics/Pickaxes/Pickaxe_CamelGram.Pickaxe_CamelGram\",\"pickaxeEKey\":\"\",\"contrailDef\":\"/BRCosmetics/Athena/Items/Cosmetics/Contrails/Contrail_PolarityWinnField.Contrail_PolarityWinnField\",\"contrailEKey\":\"\",\"shoesDef\":\"None\",\"shoesEKey\":\"\",\"mimosaDef\":\"None\",\"mimosaEKey\":\"\",\"randomDefaultCosmeticHash\":3557476875,\"scratchpad\":[],\"cosmeticStats\":[{\"statName\":\"HabaneroProgression\",\"statValue\":0},{\"statName\":\"HabaneroS31\",\"statValue\":16},{\"statName\":\"TotalVictoryCrowns\",\"statValue\":1},{\"statName\":\"TotalRoyalRoyales\",\"statValue\":0},{\"statName\":\"HasCrown\",\"statValue\":1}]}}",
						"urn:epic:member:dn_s": "Еntrарtа",
                        "Default:BattlePassInfo_j": "{\"BattlePassInfo\":{\"bHasPurchasedPass\":false,\"passLevel\":301}}",
                        "Default:PackedState_j": "{\"PackedState\":{\"subGame\":\"Athena\",\"location\":\"PreLobby\",\"gameMode\":\"None\",\"voiceChatStatus\":\"Enabled\",\"hasCompletedSTWTutorial\":true,\"hasPurchasedSTW\":true,\"platformSupportsSTW\":true,\"bDownloadOnDemandActive\":false,\"bIsPartyLFG\":false,\"bRecVoice\":false,\"bRecText\":false,\"bIsInAllSelectExperiment\":false,\"bAllowEmoteBeatSyncing\":true,\"eOSProductUserId\":\"0002314174fa484b8682fafb24d286c0\"}}",
                    },
                    "connections": [
                        {
                            "id": "b1c60df4f45a4b51b763eac539326664@prod.ol.epicgames.com/V2:Fortnite:WIN::29526DE64917CE4A791736BEB2C78A46",
							"connected_at": "2025-09-24T16:57:02.439Z",
							"updated_at": "2025-09-24T16:57:04.662Z",
							"yield_leadership": false,
							"meta": {
								"urn:epic:conn:platform_s": "WIN"
							}
                        }
                    ],
                    "revision": 1,
                    "updated_at": "2025-09-24T16:57:06.596Z",
					"joined_at": "2025-09-24T16:57:04.668Z",
					"role": "CAPTAIN"
                }
            ],
            "applicants": [],
            "meta": {
                "Default:PreferredPrivacy_s": "Private",
				"Default:AllowJoinInProgress_b": "false",
				"Default:PartyIsJoinedInProgress_b": "false",
				"Default:PartyState_s": "BattleRoyaleView",
                "urn:epic:cfg:build-id_s": "1:3:45178693",
                "Default:CustomMatchKey_s": "",
                "Default:RegionId_s": "NAE",
                "Default:PrivacySettings_j": "{\"PrivacySettings\":{\"partyType\":\"Private\",\"partyInviteRestriction\":\"AnyMember\",\"bOnlyLeaderFriendsCanJoin\":false}}",
            },
            "invites": [],
            "revision": 1,
            "intentions": []
        }
    ],
    "pending": [],
    "invites": [],
    "pings": []
}
```

_Example Response (No parties)_

```json
{
	"current": [],
	"pending": [],
	"invites": [],
	"pings": []
}
```