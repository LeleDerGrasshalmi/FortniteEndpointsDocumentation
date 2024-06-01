# EndBattleRoyaleGameV2

**Description**: `End a Battle Royale Game (V2)` \
**Profiles**: `athena` \
**Note**: `DedicatedServer ONLY`

## Body

```js
{
    "advance": [{
        "statName": "phoenixtheater_power_highlight", // The stat Name, e.g phoenixtheater_power_highlight
        "count": 1, // The count to what u want to update it
        "timestampOffset": 0 // Leave it 0
    }],
    "playlistId": "",
    "matchStats": {
        "statBucket": "",
        "matchId": "",
        "matchEndTime": "",
        "matchPlatform": "",
        "weaponStats": [{
            "weaponId": ""
        }],
        "xPStats": [{
                "stat": "",
                "count": 1,
                "Xp": 0,
                "subtype": "" // Valid: NotSet, Action, Discovery, XpToken
            }
        ],
        "bIsValid": true,
        "factionTag": ""
    },
    "totalXPAccum": 1,
    "restedXPAccum": 1,
    "friendshipXpBoost": 1,
    "cosmeticXpBoost": 1,
    "antiAddictionPlayTimeMultiplier": 1.1,
    "shouldAccumulateToProfileStats": true,
    "shouldSaveToRecentGameLists": true,
    "accolades": [{
        "accoladeDef": {}, // Yes this is missing, this is wayyy toooo much!
        "templateId": "",
        "count": 1
    }],
    "shuffledLoadoutUsed": [], // Array of strings
    "shuffledLockerUsedIndex": 0,
    "usedCosmetics": [], // Array of the cosmetics GUID
    "deletedQuestIds": [], // Array of the quests GUID
    "grantedQuestDefs": [], // Array of the quests GUID
    "secondaryXp": [{
        "type": "",
        "secondaryXp": 1
    }],
    "grantedItems": [{
        "templateId": "",
        "quantity": 1,
        "attributes": [{
            "field": "",
            "value": ""
        }]
    }],
    "grantedQuests": [{
        "templateId": "",
        "objectives": [{
            "statName": "phoenixtheater_power_highlight", // The stat Name, e.g phoenixtheater_power_highlight
            "count": 1, // The count to what u want to update it
            "timestampOffset": 0 // Leave it 0
        }],
        "expirationTime": "",
        "creationTime": ""
    }],
    "completedQuestsToClaim": [{
        "templateId": "",
        "objectives": [{
            "statName": "phoenixtheater_power_highlight", // The stat Name, e.g phoenixtheater_power_highlight
            "count": 1, // The count to what u want to update it
            "timestampOffset": 0 // Leave it 0
        }],
        "expirationTime": "",
        "creationTime": ""
    }],
    "pinnedSharedQuest": "",
    "seasonItemStates": [{
        "itemTag": "",
        "mapIconState": "" // Valid: Unknown, Found, Interacted
    }],
    "campsiteData": {
        "data_is_valid_for_mcp": true,
        "stashed_items": [{
            "item_definition_persistent_name": "",
            "item_count": 1,
            "item_level": 1,
            "item_loaded_ammo": 30
        }],
        "camp_spawn_locations": []
    },
    "victoryCrownData": {
        "has_victory_crown": true,
        "total_victory_crowns_bestowed_count": 15,
        "total_royal_royales_achieved_count": 12,
        "data_is_valid_for_mcp": true
    },
    "realitySaplingData": {
        "data_is_valid_for_mcp": true,
        "saplings": [{
            "location": {
                "X": 0,
                "Y": 0,
                "Z": 0
            },
            "rotation": {
                "Y": 0,
                "X": 0,
                "Z": 0
            },
            "nurturing_level": 0,
            "maturity_level": 0,
            "planting_time": 0,
            "last_weeding_time": 0,
            "fruit_states": [0, 0, 0]
        }]
    },
    "PlayerTimeInMatchSec": 68,
    "questAnalyticEvents": [{
        "templateId": "", // Quest id
        "state": "" // Valid: None, Granted, Claimed
    }]
}
```
