# phoenixLevelUp

**Description**: `The Reward for reaching a new Level in Ventures` \
**Operations**: [ClaimMissionAlertRewards](../Operations/ClaimMissionAlertRewards.md), [ClaimQuestReward](../Operations/ClaimQuestReward.md), [OpenCardPack](../Operations/OpenCardPack.md), [OpenCardPackBatch](../Operations/OpenCardPackBatch.md)

## Body

```js
{
    // standard profile notification content
    "type": "phoenixLevelUp",
    "primary": true,
    "client_request_id": "",

    //specific to this notification
    "level": 2,
    "loot": {
        //strangely, this is structured like a notification nested in another notification
        "type": "lootGrant",
        "primary": true,
        "client_request_id": "",

        "lootSource":"",
        "lootSourceInstance":"",
        "lootGranted": {
            "items": [
                {
                    "itemType": "Worker:workerbasic_uc_t01",
                    "itemGuid": "47bc264a-4eaf-4923-8e43-727c0eeea8d8",
                    "itemProfile": "campaign",
                    "quantity": 1
                }
                //...
            ]
        }
    }
}
```
