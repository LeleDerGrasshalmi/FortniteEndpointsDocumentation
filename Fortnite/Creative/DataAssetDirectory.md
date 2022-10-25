## Fortnite - Data Asset Directory (Asset Overwrites / external Assets)

URL: https://data-asset-directory-public-service-prod.ol.epicgames.com/api/v1/assets/Fortnite/:version/:versionCLN?appId=Fortnite \
Method: POST \
Auth Required: Yes

## Body

```json
{
  "FortPlaylistAthena": 0,
  "DAD_CosmeticItemUserOptions": 0,
  "FortPlaysetItemDefinition": 0,
  "FortAmmoItemDefinition": 0,
  "FortDecoItemDefinition": 0,
  "FortWeaponMeleeItemDefinition": 0,
  "FortWeaponMeleeDualWieldItemDefinition": 0,
  "FortWeaponRangedItemDefinition": 0,
  "FortPlaysetGrenadeItemDefinition": 0,
  "AthenaGadgetItemDefinition": 0,
  "FortPlaysetPropItemDefinition": 0,
  "FortBuildingItemDefinition": 0,
  "FortSmartBuildingItemDefinition": 0,
  "FortTrapItemDefinition": 0,
  "FortContextTrapItemDefinition": 0,
  "FortCreativeWeaponMeleeItemDefinition": 0,
  "FortEditToolItemDefinition": 0,
  "FortResourceItemDefinition": 0,
  "FortCreativeGadgetItemDefinition": 0,
  "FortCreativeActorCollection": 0,
  "FortCreativeDiscoverySurface": 0
}
```

## Parameter

**version**: the fn version (url encoded), e.g. `%2B%2BFortnite%2BRelease-20.00` \
**versionCLN**: the fn versions CLN, e.g. `19532288`

**Example final URL**: `https://data-asset-directory-public-service-prod.ol.epicgames.com/api/v1/assets/Fortnite/%2B%2BFortnite%2BRelease-20.00/19532288?appId=Fortnite`
