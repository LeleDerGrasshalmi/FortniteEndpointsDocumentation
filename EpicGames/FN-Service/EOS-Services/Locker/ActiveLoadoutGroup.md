## FN EOS Locker Service: Locker Active Loadout Group

URL: https://fngw-svc-gc-livefn.ol.epicgames.com/api/locker/v4/:deploymentId/account/:accountId/active-loadout-group \
Method: PUT \
Auth Required: Yes (`locker:{accountId} UPDATE`)

```json
{
  "loadouts": {
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
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Glider",
          "equippedItemId": "AthenaGlider:glider_id_379_gloomfemale",
          "itemCustomizations": []
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Contrails",
          "equippedItemId": "AthenaSkyDiveContrail:contrail_blazerveil",
          "itemCustomizations": []
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Shoes",
          "equippedItemId": "CosmeticShoes:shoes_breathtalepeony",
          "itemCustomizations": []
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Aura",
          "equippedItemId": "SparksAura:sparksaura_default",
          "itemCustomizations": []
        }
      ],
      "shuffleType": "DISABLED"
    },
    "CosmeticLoadout:LoadoutSchema_Vehicle_SUV": {
      "loadoutSlots": [
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_Body_SUV",
          "itemCustomizations": []
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_Skin_SUV",
          "itemCustomizations": []
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_Wheel_SUV",
          "equippedItemId": "VehicleCosmetics_Wheel:wheel_rl152sport",
          "itemCustomizations": [
            {
              "channelTag": "Vehicle.Painted",
              "variantTag": "Vehicle.Painted.Cobalt",
              "additionalData": ""
            }
          ]
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_DriftSmoke_SUV",
          "equippedItemId": "VehicleCosmetics_DriftTrail:id_drifttrail_standard",
          "itemCustomizations": []
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_Booster_SUV",
          "equippedItemId": "VehicleCosmetics_Booster:id_booster_standard",
          "itemCustomizations": []
        }
      ],
      "shuffleType": "DISABLED"
    }
  }
}
```

## Path Parameters

`deploymentId`: The Deployment Id from env configuration, for `live-fn` it is `62a9473a2dca46b29ccf17577fcf42d7` <br/>
`accountId`: Your Account Id

---

_Example Response_

```json
{
  "deploymentId": "62a9473a2dca46b29ccf17577fcf42d7",
  "accountId": "b1c60df4f45a4b51b763eac539326664",
  "athenaItemId": "d4a6db65-c223-4358-a67e-f0c519094b6b",
  "creationTime": "2024-11-02T15:30:13.693713773Z",
  "updatedTime": "2024-12-17T19:46:25.946968957Z",
  "loadouts": {
    "CosmeticLoadout:LoadoutSchema_Vehicle_SUV": {
      "loadoutSlots": [
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_Body_SUV",
          "itemCustomizations": []
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_Skin_SUV",
          "itemCustomizations": []
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_Wheel_SUV",
          "equippedItemId": "VehicleCosmetics_Wheel:wheel_rl152sport",
          "itemCustomizations": [
            {
              "channelTag": "Vehicle.Painted",
              "variantTag": "Vehicle.Painted.Cobalt",
              "additionalData": ""
            }
          ]
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_DriftSmoke_SUV",
          "equippedItemId": "VehicleCosmetics_DriftTrail:id_drifttrail_standard",
          "itemCustomizations": []
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Vehicle_Booster_SUV",
          "equippedItemId": "VehicleCosmetics_Booster:id_booster_standard",
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
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Glider",
          "equippedItemId": "AthenaGlider:glider_id_379_gloomfemale",
          "itemCustomizations": []
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Contrails",
          "equippedItemId": "AthenaSkyDiveContrail:contrail_blazerveil",
          "itemCustomizations": []
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Shoes",
          "equippedItemId": "CosmeticShoes:shoes_breathtalepeony",
          "itemCustomizations": []
        },
        {
          "slotTemplate": "CosmeticLoadoutSlotTemplate:LoadoutSlot_Aura",
          "equippedItemId": "SparksAura:sparksaura_default",
          "itemCustomizations": []
        }
      ],
      "shuffleType": "DISABLED"
    }
  },
  "shuffleType": "DISABLED"
}
```
