# SetHeroCosmeticVariants

**Description**: `Set the Variants for a Hero and his Backpack` \
**Profiles**: `campaign`

## Body

```js
{
    "heroItem": "", // Hero item GUID
    "outfitVariants": [{
        "channel": "Parts", // Variant channel
        "active": "CampaignHero.Tier2.Legendary", // Variant tag
        "owned": [] // Can be left as an empty array
    }],
    "backblingVariants": [{
        "channel": "", // Variant channel
        "active": "", // Variant tag
        "owned": [] // Can be left as an empty array
    }]
}
```
