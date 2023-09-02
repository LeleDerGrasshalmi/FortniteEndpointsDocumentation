# UpgradeHero

**Description**: `Upgrades a hero (+ pet in old versions)` \
**Profiles**: `profile0`

## Body

```js
{
    "heroItemId": "", // GUID of Hero to Upgrade
    "bIsInPit": false, // Whether the Hero is in the Pit
    "potionItems": [
        {
            "upgradeType": "", // Template ID for Potion
            "numUpgrades": 0 // Number of Upgrades to Apply
        }
    ],
    "weaponUpgrades": [
        {
            "upgradeType": "", // Type of Upgrade (e.g. Weapon/Armor Level/Stars)
            "numUpgrades": 0 // Number of Upgrades to Apply
        }
    ]
}
```
