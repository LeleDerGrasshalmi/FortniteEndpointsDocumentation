# EndBattleRoyaleGame

**Description**: `End a Battle Royale Game` \
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
    "AntiAddictionPlayTimeMultiplier": 1.1,
    "shouldAccumulateToProfileStats": true,
    "shouldSaveToRecentGameLists": true,
    "accolades": [{
        "accoladeDef": {}, // Yes this is missing, this is wayyy toooo much!
        "templateId": "",
        "count": 1
    }],
    "shuffledLoadoutUsed": [], // Array of strings
    "shuffledLockerUsedIndex": 0,
    "grantedQuestDefs": [], // Array of the quests guid
    "secondaryXp": [{
        "type": "",
        "secondaryXp": 1
    }]
}
```
