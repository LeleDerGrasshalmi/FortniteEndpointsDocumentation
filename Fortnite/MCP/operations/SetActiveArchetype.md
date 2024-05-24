# SetActiveArchetype

**Description**: `Sets the active archetype (e.g. Primary Vehicle)` \
**Profiles**: `athena`

## Body

```js
{
    "archetypeGroup": "", // e.g. CosmeticArchetype:LoadoutArchetype_Vehicles
    "archetype": "" // e.g. Vehicle.Archetype.SportsCar
}
```

_An example of the profile stat affected by this request_

```js
{
    "stats": {
        "attributes": {
            "loadout_archetype_values": {
                "CosmeticArchetype:LoadoutArchetype_Vehicles": "Vehicle.Archetype.SportsCar"
            }
        }
    }
}
```
