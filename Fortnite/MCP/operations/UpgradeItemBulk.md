# UpgradeItemBulk

**Description**: `Evolve an Item (upgrade its tier)` \
**Profiles**: `campaign`

## Body
```js
{
    "targetItemId": "", //guid of the item
    "desiredLevel": 10, //desired Level to upgrade to
    "desiredTier": "no_tier", //the tier
    "conversionRecipeIndexChoice": -1 //idk, leave like this ig
}
```
