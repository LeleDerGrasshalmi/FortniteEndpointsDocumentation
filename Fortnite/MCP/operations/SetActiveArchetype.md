# SetActiveArchetype

**Description**: `Sets the active archetype (e.g. Primary Vehicle)` \
**Profiles**: `athena`

## Body

```js
{
    "archetypeGroup": "", // Check available values below
    "archetype": "" // Check available values below
}
```

`archetypeGroup` (which loadout archetype to modify)
- `CosmeticArchetype:LoadoutArchetype_Vehicles`

`archetype` (which archetype group tag to set)
- `Vehicle.Archetype.SUV`
- `Vehicle.Archetype.SportsCar`

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
