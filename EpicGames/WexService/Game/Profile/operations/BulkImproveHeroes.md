# BulkImproveHeroes

**Description**: `Applies upgrades to heroes in bulk (used by party suggestion)` \
**Profiles**: `profile0`

## Body

```js
{
    "detail": [
        {
            "heroItemId": "", // GUID of Hero to Upgrade
            "potionItems": [
                {
                    "upgradeType": "", // Template ID for Potion
                    "numUpgrades": 0 // Number of Upgrades to Apply
                }
            ],
            "weaponUpgrades": [
                {
                    "upgradeType": "", // Type of Upgrade (e.g. WeaponLevel or WeaponStars)
                    "numUpgrades": 0 // Number of Upgrades to Apply
                }
            ],
            "numLevelUps": 0 // Number of Times to Level Up Hero
        }
    ]
}
```
