# SetCosmeticLockerSlots

**Description**: `Set multiple Cosmetics in a specified Locker` \
**Profiles**: `athena`, `campaign`

## Body

```js
{
    "lockerItem": "", // The Locker Item GUID
    "loadoutData": [{
        "category": "", // The category in which the item should be set, e.g. Character, Backpack, Dance
        "itemToSlot": "AthenaCharacter:CID_029_Athena_Commando_F_Halloween", // The cosmetic to equip (see formating in the example!)
        "slotIndex": 0 // Normally its 0, -1 to equip a wrap on every slot, else (0-5 on emotes stuff, 0-6 on wraps stuff)
        "variantUpdates": []
    }]
}
```
\
**variantUpdates format**

```js
{
    "channel": "Material", // Variant channel
    "active": "Mat2", // Variant tag
    "owned": [] // Can be left as an empty array
}
```
