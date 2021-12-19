# UnlockRewardNode

**Description**: `unlocks a reward by its nodeId (used in winterfest)` \
**Profiles**: `athena`

## Body
```js
{
    "nodeId": "ERG.Node.A.7", //the rewards nodeId you want to open
    "rewardGraphId": "AthenaRewardGraph:s19_winterfest", //the RewardGraphs GUID
    "rewardCfg": "" //can be left empty
}
```
