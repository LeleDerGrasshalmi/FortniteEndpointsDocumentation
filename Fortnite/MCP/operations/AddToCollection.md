# AddToCollection

**Description**: `Adds an item to the collection` \
**Profiles**: `collections` \
**Note**: `DedicatedServer ONLY`

## Body
```js
{
    "category": "", //item guid or templateId
    "variant": "", //variant tag
    "contextTags": [],
    "properties": {}, //for fishes: weight(float), length(float) || for npcs: questsGiven(int), questsCompleted(int), encounterTypeFlags(char)
    "seenState": "", //valid: Unknown, New, Known, NewlyCollected, Collected, NewBest, NewRecord, NewLocation, NewlyCompleted, Complete
    "count": 1
}
```
