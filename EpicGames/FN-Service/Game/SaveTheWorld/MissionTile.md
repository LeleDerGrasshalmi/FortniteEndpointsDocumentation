## FN Service - STW Tile

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/game/v2/world/tile/:TheaterId/:TileTag \
Method: GET \
Auth Required: Yes

## Path Parameters

`theaterId`: The Theater GUID. Example: Hestia `C4C2925C466832846A042E97F00FE5CF` <br/>
`tileTag`: The Tile Tag. Example: `Theater.Tile.Homebase`

---

_Example Response_

```json
{
    "missionGuid": "d0d9fdea-f463-4f3a-b1ab-ac886b22aee2",
    "missionRewards": {
        "tierGroupName": "Mission_Select_T01",
        "items": [
            {
                "itemType": "CardPack:zcp_eventscaling_t01",
                "quantity": 1
            }
        ]
    },
    "bonusMissionRewards": {
        "tierGroupName": "Mission_Select_Bonus_T01",
        "items": [
            {
                "itemType": "CardPack:zcp_eventscaling_t01",
                "quantity": 1
            }
        ]
    },
    "overrideMissionRewards": {},
    "missionGenerator": "/STW_HestiaBeauty/Mission/MissionGen/MissionGen_HestiaBeauty.MissionGen_HestiaBeauty_C",
    "missionDifficultyInfo": {
        "dataTable": "/Script/Engine.DataTable'/SaveTheWorld/Balance/DataTables/GameDifficultyGrowthBounds.GameDifficultyGrowthBounds'",
        "rowName": "Theater_HestiaBeauty"
    },
    "tileIndex": 0,
    "availableUntil": "2026-07-20T00:00:00.000Z"
}
```
