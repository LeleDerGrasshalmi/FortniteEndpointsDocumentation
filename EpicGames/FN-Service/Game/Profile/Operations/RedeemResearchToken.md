# RedeemResearchToken

**Description**: `Research the schematic of a looted weapon` ([This](https://imgur.com/a/pal4BT6)) \
**Profiles**: `campaign`

## Body

```js
{
    "index": 1 // Selected schematic index
}
```

Below is an example of the `campaignresearchtoken` item in the `campaign` profile. The index in the body of the request is the index of the selected item from `items_for_schematic_creation_data`:

```json
"fdabc770-907b-4fe8-921d-e0eebd32c529" : {
    "templateId" : "Token:campaignresearchtoken",
    "attributes" : {
        "items_for_schematic_creation_data" : [
            {
                "itemId" : "Weapon:wid_sniper_auto_sr_ore_t05",
                "itemPerks" : ["Alteration:aid_att_reloadspeed_ranged_t05", "Alteration:aid_att_stability_t05", "Alteration:aid_ele_energy_t05", "Alteration:aid_att_critdamage_t05", "Alteration:aid_conditional_slowed_dmgbonus_t05", "Alteration:aid_g_ranged_headshotstreak_dmgbonus_v2"],
                "itemLevel" : 40
            },
            {
                "itemId" : "Weapon:wid_assault_doubleshot_sr_ore_t05",
                "itemPerks" : ["Alteration:aid_att_critdamage_t05", "Alteration:aid_att_maxdurability_t05", "Alteration:aid_ele_nature_t05", "Alteration:aid_att_headshotdamage_t05", "Alteration:aid_conditional_boss_dmgbonus_t05", "Alteration:aid_g_ranged_headshotstreak_dmgbonus_v2"],
                "itemLevel" : 40
            },
            {
                "itemId" : "Trap:tid_floor_flamegrill_vr_t05",
                "itemPerks" : [],
                "itemLevel" : 40
            },
            {
                "itemId" : "Weapon:wid_shotgun_semiauto_vr_crystal_t05",
                "itemPerks" : ["Alteration:aid_att_critdamage_t04", "Alteration:aid_att_magazinesize_t05", "Alteration:aid_ele_water_t05", "Alteration:aid_att_critchance_t05", "Alteration:aid_conditional_slowed_dmgbonus_t05"],
                "itemLevel" : 40
            }
        ],
        "level" : 1,
        "num_awarded_items_for_schematic_creation" : 1
    },
    "quantity" : 1
}
```
