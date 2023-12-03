# PutModularCosmeticLoadout

**Description**: `Set the complete cosmetic loadout` \
**Profiles**: `athena`

## Body

```js
{
    "loadoutType": "CosmeticLoadout:LoadoutSchema_Platform", // e.g. fuck it
    "presetId": 0, // loadout index
    "loadoutData": "" // stringified json locker data, see below
}
```

Stringified Data has the following format

```js
{
    "slots": [{
            "slot_template": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Banner_Icon",
            "equipped_item": "HomebaseBannerIcon:standardbanner15"
        },
        {
            "slot_template": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Banner_Color",
            "equipped_item": "HomebaseBannerColor:defaultcolor37"
        },
        {
            "slot_template": "CosmeticLoadoutSlotTemplate:LoadoutSlot_LobbyMusic",
            "equipped_item": "AthenaMusicPack:musicpack_000_stw_default"
        },
        {
            "slot_template": "CosmeticLoadoutSlotTemplate:LoadoutSlot_LoadingScreen",
            "equipped_item": "AthenaLoadingScreen:loadingscreen_bites"
        }
    ]
}
```
