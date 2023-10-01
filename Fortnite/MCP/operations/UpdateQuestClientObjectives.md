# UpdateQuestClientObjectives

**Description**: `Update a Objective for a Quest (Bulk)` Note: Used for quests completable in the lobby \
**Profiles**: `campaign`, `athena`

## Body

```js
{
    "advance": [{
        "statName": "phoenixtheater_power_highlight", // The stat Name, e.g phoenixtheater_power_highlight
        "count": 1, // The count to what u want to update it
        "timestampOffset": 0 // Leave it 0, this is related to the difference between Local and UTC Time
    }]
}
```
