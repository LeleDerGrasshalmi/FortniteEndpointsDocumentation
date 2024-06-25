# MarkCollectedItemsSeen

**Description**: `Mark Collection Items as seen (Bulk)` \
**Profiles**: `collections`

## Body

```js
{
    "variants": [{
        "category": "", // Category Template Id, e.g. CollectableCharacter:tandem, CollectableCharacter:boss, CollectablePlayerAugment:collection
        "variant": "" // The Variant Gameplaytag, e.g. AISpawnerData.Type.Tandem.SpaceChimp, PlayerAugment.Collection.PartyTime, Fish.Angler.PurpleOrange
    }]
}
```
