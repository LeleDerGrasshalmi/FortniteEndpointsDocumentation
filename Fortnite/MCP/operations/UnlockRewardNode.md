# UnlockRewardNode

**Description**: `unlocks a reward by its nodeId (used in winterfest)` \
**Profiles**: `athena`

## Body
```js
{
    "nodeId": "{nodeId}", //the rewards nodeId you want to open
    "rewardGraphId": "{guid}", //the RewardGraphs GUID
    "rewardCfg": "" //can be left empty
}
```
