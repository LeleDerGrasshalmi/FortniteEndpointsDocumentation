# SetLoadoutShuffleEnabled
**Description**: `Enables shuffle for the specified loadout section.` \
**Profile**: `athena`

## Body

```js
{
    "loadoutType": ":LoadoutSchema_Jam", // The Loadout Section, see 'PutModularCosmeticLoadout' operation for possible values
    "bEnabled": false // Boolean
}
```
