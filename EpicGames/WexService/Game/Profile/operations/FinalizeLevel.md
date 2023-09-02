# FinalizeLevel

**Description**: `Claim rewards for an active level` \
**Profiles**: `levels`

## Body

```js
{
    "levelItemId": "", // Level Instance GUID
    "levelElement": "", // Main Level Element (new versions only)
    "claimDepth": "", // Number of Rooms Completed
    "claimedItems": [
        {
            "itemTemplateId": "", // TemplateID of Item
            "quantity": 0 // Quantity of Item (enforced by anticheat in later versions)
        }
    ],
    "seenCharacters": [
        "" // TemplateID of Characters Seen
    ],
    "postBattleResults": { // New versions only
        "defeatedEnemyMap": {
            "Nature": 0 // Number of Enemies Defeated per Element
        },
        "uniqueHeroesDefeated": [
            "" // GUID of Heroes Defeated
        ],
        "uniqueEnemiesDefeated": [
            "", // Template ID:RoomDepth=0 Slot=0 SideRoom=0
        ]
    },
    "battleMetaData": "Bs/xxx/xx==", // Encoded AntiCheat Data (later versions only; yet to be defeated)
    "dailyQuestZoneType": 0, // Zone Type of Daily Quest (new versions only)
    "partyItemId": "", // 8 Characters of something cool (new versions only)
    "bShouldGiveBonus": false // Should give bonus rewards (e.g. for first time completion) (new versions only)
}
```
