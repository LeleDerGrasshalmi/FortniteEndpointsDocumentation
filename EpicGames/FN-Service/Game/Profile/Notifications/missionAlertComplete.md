# missionAlertComplete

**Description**: `The claimed Mission Alert Rewards` \
**Operations**: [ClaimMissionAlertRewards](../Operations/ClaimMissionAlertRewards.md)

## Body

```js
{
    // standard profile notification content
    "type": "missionAlertComplete",
    "primary": true,
    "client_request_id": "",

    //specific to this notification
    "lootGranted": {
        "tierGroupName": "MissionAlert_Seasonal_PassiveMiniboss:11",
        "items": [
            {
                "itemType": "AccountResource:currency_mtxswap",
                "itemGuid": "",
                "itemProfile": "campaign",
                "quantity": 50
            }
            //...
        ]
    }
}
```
