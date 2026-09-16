# questClaim

**Description**: `The rewards of a claimed Quest` \
**Operations**: [ClaimQuestReward](../Operations/ClaimQuestReward.md), [ExecuteTerminalCommand](../Operations/ExecuteTerminalCommand.md),

## Body

```js
{
    // standard profile notification content
    "type": "questClaim",
    "primary": true,
    "client_request_id": "",

    //specific to this notification
    "questId": "Quest:quest_s42_cosmicthunder_00_promo_q22"
    "loot": {
        "items": [
        {
            "itemType": "MagpieEntitlementReward:magpiereward_jonesy_gold_sprite",
            "itemGuid": "d9d56ffb-c1d0-46c2-9cf8-d2cbb211b061",
            "itemProfile": "athena",
            "attributes": {},
            "quantity": 1
        }
            //...
        ]
    },
    // when claiming multiple quests at once
    "questsAndRewards": [{
            "questId": "Quest:quest_s28_winterfest_dailygift_q01",
            "loot": {
                "items": [{
                    "itemType": "AthenaBackpack:backpack_wintergift",
                    "itemGuid": "dbf80ea6-fa45-490b-a747-24ee705263a5",
                    "itemProfile": "athena",
                    "quantity": 1
                }]
            }
        }
    ]
}
```
