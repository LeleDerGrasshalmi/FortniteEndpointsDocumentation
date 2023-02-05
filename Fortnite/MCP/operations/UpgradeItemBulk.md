# UpgradeItemBulk

**Description**: `Evolve an Item (upgrade its tier)` \
**Profiles**: `campaign`

## Body
```js
{
    "targetItemId": "", // Item GUID
    "desiredLevel": 10, // Desired Level to upgrade to
    "desiredTier": "no_tier", // The tier
    "conversionRecipeIndexChoice": -1 // Idk, leave like this ig
}
```
