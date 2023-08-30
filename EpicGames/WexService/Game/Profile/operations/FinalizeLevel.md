# FinalizeLevel

**Description**: `Claim rewards for an active level` \
**Profiles**: `levels`

## Body

```js
{
    "levelItemId": "", // Level Instance GUID
    "levelElement": "", // Main Level Element
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
    "postBattleResults": {
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
    "dailyQuestZoneType": 0, // Zone Type of Daily Quest
    "partyItemId": "", // 8 Characters of something cool
    "bShouldGiveBonus": false // Should give bonus rewards (e.g. for first time completion)
}
```
