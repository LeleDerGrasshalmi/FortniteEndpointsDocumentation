# EndBattleRoyaleGameV2

**Description**: `End a Battle Royale Game (V2)` \
**Profiles**: `athena` \
**Note**: `DedicatedServer ONLY`

## Body
```js
{
    "advance": [{
        "statName": "phoenixtheater_power_highlight", //the stat Name, e.g phoenixtheater_power_highlight
        "count": 1, //the count to what u want to update it
        "timestampOffset": 0 //leave it 0
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
                "subtype": "" //valid: NotSet, Action, Discovery, XpToken
            }
        },
        "bIsValid": true,
        "factionTag": ""
    },
    "totalXPAccum": 1,
    "restedXPAccum": 1,
    "friendshipXpBoost": 1,
    "cosmeticXpBoost": 1,
    "AntiAddictionPlayTimeMultiplier": 1.1,
    "shouldAccumulateToProfileStats": true,
    "shouldSaveToRecentGameLists": true,
    "accolades": [{
        "accoladeDef": {}, //yes this is missing, this is wayyy toooo much!
        "templateId": "",
        "count": 1
    }],
    "shuffledLoadoutUsed": [], //array of strings
    "shuffledLockerUsedIndex": 0,
    "deletedQuestIds": [], //array of the quests guid
    "grantedQuestDefs": [], //array of the quests guid
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
    "grantedTransientQuests": [{
        "templateId": "",
        "objectives": [{
            "statName": "phoenixtheater_power_highlight", //the stat Name, e.g phoenixtheater_power_highlight
            "count": 1, //the count to what u want to update it
            "timestampOffset": 0 //leave it 0
        }],
        "expirationTime": "",
        "creationTime": ""
    }],
    "pinnedSharedQuest": "",
    "seasonItemStates": [{
        "itemTag": "",
        "mapIconState": "" //valid: Unknown, Found, Interacted
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
    "PlayerTimeInMatchSec": 68
}
```
