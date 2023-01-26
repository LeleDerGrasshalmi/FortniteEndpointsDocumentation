# SetHeroCosmeticVariants

**Description**: `Set the Variants for a Hero/Hero's Backpack` \
**Profiles**: `campaign`

## Body
```js
{
    "heroItem": "", // Hero item GUID
    "outfitVariants": [],
    "backblingVariants": []
}
```
\
**Variants format**
```js
{
    "channel": "Parts", // Variant channel
    "active": "CampaignHero.Tier2.Legendary", // Variant tag
    "owned": [] // Can be left as an empty array
}
```
