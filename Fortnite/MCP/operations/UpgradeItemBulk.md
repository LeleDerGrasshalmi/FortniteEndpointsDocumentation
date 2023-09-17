# UpgradeItemBulk

**Description**: `Evolve an Item (upgrade its Tier)` \
**Profiles**: `campaign`

## Body

```js
{
    "targetItemId": "", // Item GUID
    "desiredLevel": 10, // Desired Level to upgrade to
    "desiredTier": "no_tier", // The Tier, 'no_tier' or Lowercased Romanian Numbers
    "conversionRecipeIndexChoice": -1 // Index if there is more than 1 option (e.g. Obsidian vs Shadowshard)
}
```
