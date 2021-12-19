# SetCosmeticLockerSlot

**Description**: `Set a Cosmetic with a specified index to in a specified LockerLocker` \
**Profiles**: `athena`

## Body
```js
{
    "lockerItem": "{lockerItemGUID}", //the Locker Items GUID
    "category": "{category}", //the categiry in which the item should be set, e.g. Character, Backpack, Dance
    "itemToSlot": "AthenaCharacter:CID_029_Athena_Commando_F_Halloween", //the cosmetic to equip (see formating in the example!)
    "slotIndex": 0, //normally its 0, -1 to equip a wrap on every slot, else (0-5 on emotes stuff, 0-6 on wraps stuff)
    "variantUpdates": [],
    "optLockerUseCountOverride": 0 //idk
}
```
\
**variantUpdates format**
```js
{
    "channel": "Material", //variant channel
    "active": "Mat2", //variant tag
    "owned": [] //can be left as an empty array
}
```
