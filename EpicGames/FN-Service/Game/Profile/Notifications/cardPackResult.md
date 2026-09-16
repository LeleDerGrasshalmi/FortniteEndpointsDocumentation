# cardPackResult

**Description**: `The contents of one or many CardPacks` \
**Operations**: [OpenCardPack](../Operations/OpenCardPack.md), [OpenCardPackBatch](../Operations/OpenCardPackBatch.md)

## Body

```js
{
    // standard profile notification content
    "type": "cardPackResult",
    "primary": true,
    "client_request_id": "",

    //specific to this notification
    "lootGranted": {
        "tierGroupName": "CardPack_Event_Persistent_Lunar", //absent when using OpenCardPackBatch
        "items": [
            {
                "itemType": "Worker:workerbasic_uc_t01",
                "itemGuid": "47bc264a-4eaf-4923-8e43-727c0eeea8d8",
                "itemProfile": "campaign",
                "quantity": 1
            }
            //...
        ]
    },
    "displayLevel": 0,
    "tierGroupName": "CardPack_Event_Persistent_Lunar", //absent when using OpenCardPackBatch
    "tier": -1,
    "overrideTier": -1
}
```
