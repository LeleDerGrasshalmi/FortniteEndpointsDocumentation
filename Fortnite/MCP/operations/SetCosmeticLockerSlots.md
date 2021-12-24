# SetCosmeticLockerSlots

**Description**: `Set multible Cosmetics in a specified Locker (unkown if the variantUpdates parameter exists!)` \
**Profiles**: `athena`, `campaign`

## Body
```js
{
    "lockerItem": "{lockerItemGUID}", //the Locker Items GUID
    "loadoutData": [{
        "slotName": "{category}", //the category in which the item should be set, e.g. Character, Backpack, Dance
        "itemToSlot": "AthenaCharacter:CID_029_Athena_Commando_F_Halloween", //the cosmetic to equip (see formating in the example!)
        "indexWithinSlot": 0 //normally its 0, -1 to equip a wrap on every slot, else (0-5 on emotes stuff, 0-6 on wraps stuff)
    }]
}
```
