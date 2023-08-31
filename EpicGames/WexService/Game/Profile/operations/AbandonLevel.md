# AbandonLevel

**Description**: `Abandon an active level without claiming rewards` \
**Profiles**: `levels`

## Body

```js
{
    "levelItemId": "", // Level Instance GUID
    "depthCompleted": 0, // Number of Rooms Completed
    "levelElement": "", // Main Level Element
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
    "dailyQuestZoneType": 0 // Zone Type of Daily Quest
}
```
