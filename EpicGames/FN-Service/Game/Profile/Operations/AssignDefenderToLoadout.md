# AssignDefenderToLoadout

**Description**: `Assigns a Defender to a Defender slot in a Loadout` \
**Profiles**: `campaign`
### Note
As of v40.00 this operation is unusable, as no one has unlocked any of the 3 Defender slots for their Loadout yet

## Body

```js
{
    "defenderId": "", // Defender Item GUID
    "loadoutId": "", // Loadout Item GUID
    "slotName": "" // Slots Name, valid: DefenderSlot(1-3) e.g. DefenderSlot2
}
```
