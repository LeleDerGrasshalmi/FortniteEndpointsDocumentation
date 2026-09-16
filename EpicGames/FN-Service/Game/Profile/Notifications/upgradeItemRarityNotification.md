# upgradeItemRarityNotification

**Description**: `The result of the Rarity Upgrade` \
**Operations**: [UpgradeItemRarity](../Operations/UpgradeItemRarity.md)

## Body

```js
{
    // standard profile notification content
    "type": "upgradeItemRarityNotification",
    "primary": true,
    "client_request_id": "",

    //specific to this notification
    "itemsGranted": [
        {
            "itemType": "Worker:workerbasic_vr_t01",
            "itemGuid": "d9d56ffb-c1d0-46c2-9cf8-d2cbb211b061",
            "itemProfile": "campaign",
            "attributes": {},
            "quantity": 1
        }
        //...
    ]
}
```
