# PutModularCosmeticLoadout

**Description**: `Set the cosmetic loadout for a certain loadout type` \
**Profiles**: `athena`

## Body

```js
{
    "loadoutType": "CosmeticLoadout:LoadoutSchema_Platform", // check known list below..
    "presetId": 0, // loadout index
    "loadoutData": "" // stringified json, see schema below
}
```

Stringified Data has the following format.

> When setting no `equipped_item` the slot will be empty.

```js

{
    "slots": [{
            "slot_template": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Banner_Icon", // see types below...
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
            "equipped_item": "AthenaLoadingScreen:loadingscreen_bites",
			"customization_info": [ // styles (copied from a car section to showcase the schema)
				{
					"channel_tag": "Vehicle.Painted",
					"variant_tag": "Vehicle.Painted.None"
				}
			]
        }
    ],
    "display_name": "my new name" // optional to update the loadouts name
}
```

`loadoutType` (which locker type/section to edit)

- `CosmeticLoadout:LoadoutSchema_Character` (Skins)
- `CosmeticLoadout:LoadoutSchema_Emotes` (Emotes)
- `CosmeticLoadout:LoadoutSchema_Wraps` (Wraps)
- `CosmeticLoadout:LoadoutSchema_Platform` (Lobby)
- `CosmeticLoadout:LoadoutSchema_Sparks` (Instruments)
- `CosmeticLoadout:LoadoutSchema_Jam` (Jam Tracks)
- `CosmeticLoadout:LoadoutSchema_Vehicle` (Cars)

`slot_template` (depending on loadout type you can use the slot templates)

- `CosmeticLoadout:LoadoutSchema_Character`

  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Character`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Backpack`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Pickaxe`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Glider`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Contrails`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Aura`

- `CosmeticLoadout:LoadoutSchema_Emotes`

  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Emote_0`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Emote_1`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Emote_2`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Emote_3`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Emote_4`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Emote_5`

- `CosmeticLoadout:LoadoutSchema_Wraps`

  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Wrap_0`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Wrap_1`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Wrap_2`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Wrap_3`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Wrap_4`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Wrap_5`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Wrap_6`

- `CosmeticLoadout:LoadoutSchema_Platform`

  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Banner_Icon`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Banner_Color`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_LobbyMusic`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_LoadingScreen`

- `CosmeticLoadout:LoadoutSchema_Sparks`

  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Bass`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Guitar`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Drum`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Keyboard`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Microphone`

- `CosmeticLoadout:LoadoutSchema_Jam`

  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_JamSong0`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_JamSong1`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_JamSong2`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_JamSong3`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_JamSong4`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_JamSong5`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_JamSong6`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_JamSong7`

- `CosmeticLoadout:LoadoutSchema_Vehicle`

  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_Body`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_Booster`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_DriftSmoke`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_Wheel`
  - `CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_Skin`
