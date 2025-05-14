# SetSeasonPassAutoClaim

**Description**: `Enable or Disable the Auto-Claim Feature in specified passes.` \
**Profiles**: `athena`

## Body

```js
{
    "seasonIds": ["br"], // br (Battle Royale Pass), figment (OG), musicpass (Festival), juno (LEGO)
    "bEnabled": true // Whether to use the Auto-Claim feature
}
```
