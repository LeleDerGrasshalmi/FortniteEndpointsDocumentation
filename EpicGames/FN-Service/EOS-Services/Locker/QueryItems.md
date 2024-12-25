## FN EOS Locker Service: Query Items

URL: https://fngw-svc-gc-livefn.ol.epicgames.com/api/locker/v4/:deploymentId/account/:accountId/items \
Method: GET \
Auth Required: Yes (`locker:items`)

## Path Parameters

`deploymentId`: The Deployment Id from env configuration, for `live-fn` it is `62a9473a2dca46b29ccf17577fcf42d7` <br/>
`accountId`: Your Account Id

---

_Example Response (shortened)_

```json
{
  "activeLoadoutGroup": {
    "deploymentId": "62a9473a2dca46b29ccf17577fcf42d7",
    "accountId": "b1c60df4f45a4b51b763eac539326664",
    "athenaItemId": "d4a6db65-c223-4358-a67e-f0c519094b6b",
    "creationTime": "2024-11-02T15:30:13.693713773Z",
    "updatedTime": "2024-12-15T20:19:12.879908946Z",
    "loadouts": {
      "CosmeticLoadout:LoadoutSchema_Emotes": {
        "loadoutSlots": [
          {
            "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Emote_3",
            "equippedItemId": "AthenaDance:eid_enrapture",
            "itemCustomizations": [
              {
                "channelTag": "TagDriven",
                "variantTag": "Stage1",
                "additionalData": ""
              }
            ]
          },
          {
            "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Emote_4",
            "equippedItemId": "AthenaDance:eid_guitar_shakecrunch",
            "itemCustomizations": [
              {
                "channelTag": "ProfileLoadout",
                "variantTag": "ProfileLoadout",
                "additionalData": ""
              }
            ]
          },
          {
            "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Emote_5",
            "equippedItemId": "AthenaDance:eid_laugh",
            "itemCustomizations": []
          }
        ],
        "shuffleType": "DISABLED"
      },
      "CosmeticLoadout:LoadoutSchema_Character": {
        "loadoutSlots": [
          {
            "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Character",
            "equippedItemId": "AthenaCharacter:character_rosedepth_seed",
            "itemCustomizations": [
              {
                "channelTag": "Progressive",
                "variantTag": "Stage2",
                "additionalData": ""
              }
            ]
          },
          {
            "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Backpack",
            "equippedItemId": "AthenaBackpack:backpack_blazerveil",
            "itemCustomizations": []
          },
          {
            "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Pickaxe",
            "equippedItemId": "AthenaPickaxe:pickaxe_blazerveil",
            "itemCustomizations": []
          }
        ],
        "shuffleType": "DISABLED"
      }
    },
    "shuffleType": "DISABLED"
  },
  "loadoutGroupPresets": [],
  "loadoutPresets": [
    {
      "deploymentId": "62a9473a2dca46b29ccf17577fcf42d7",
      "accountId": "b1c60df4f45a4b51b763eac539326664",
      "loadoutType": "CosmeticLoadout:LoadoutSchema_Character",
      "presetId": "0001",
      "presetIndex": 1,
      "athenaItemId": "b4224ae3-69b6-4bc0-9f75-3ecbfb0568d0",
      "creationTime": "2024-08-24T12:12:06.974010475Z",
      "updatedTime": "2024-08-24T12:12:06.974010475Z",
      "loadoutSlots": [
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Character",
          "equippedItemId": "AthenaCharacter:cid_313_athena_commando_m_kpopfashion"
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Backpack",
          "equippedItemId": "AthenaBackpack:bid_430_galileospeedboat_9rxe3"
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Pickaxe",
          "equippedItemId": "AthenaPickaxe:pickaxe_id_315_banefemale1h"
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Glider",
          "equippedItemId": "AthenaGlider:glider_id_146_masako"
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Contrails",
          "equippedItemId": "AthenaSkyDiveContrail:trails_id_037_glyphs"
        }
      ],
      "displayName": "Ikonik"
    }
  ]
}
```
