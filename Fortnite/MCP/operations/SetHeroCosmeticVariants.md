# SetHeroCosmeticVariants

**Description**: `Set the Variants for a Hero/Hero's Backpack` \
**Profiles**: `campaign`

## Body
```js
{
    "heroItem": "", //hero item guid
    "outfitVariants": [],
    "backblingVariants": []
}
```
\
**Variants format**
```js
{
    "channel": "Parts", //variant channel
    "active": "CampaignHero.Tier2.Legendary", //variant tag
    "owned": [] //can be left as an empty array
}
```
