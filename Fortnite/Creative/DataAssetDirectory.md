## Fortnite - Data Asset Directory: Assets (Gamefile Overwrites)

URL: https://data-asset-directory-public-service-prod.ol.epicgames.com/api/v1/assets/Fortnite/:version/:versionCLN?appId=Fortnite \
Method: POST \
Auth Required: Yes (`dad:fortnite:assets:* READ`)

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

## Path Parameters

`version`: the fn version (url encoded), e.g. `%2B%2BFortnite%2BRelease-20.00` <br/>
`versionCLN`: the fn versions CLN, e.g. `19532288`

---

_Example Response (heavily shortened)_

```json
{
  "FortCreativeDiscoverySurface": {
    "meta": {
      "promotion": 23
    },
    "assets": {
      "CreativeDiscoverySurface_Library": {
        "meta": {
          "revision": 2,
          "headRevision": 2,
          "revisedAt": "2023-04-26T15:02:18.478Z",
          "promotion": 1,
          "promotedAt": "2023-05-02T08:20:28.948Z"
        },
        "assetData": {
          "AnalyticsId": "",
          "TestCohorts": [
            {
              "AnalyticsId": "",
              "CohortSelector": "Always",
              "PlatformBlacklist": [],
              "CountryCodeBlocklist": [],
              "ContentPanels": [],
              "PlatformWhitelist": [],
              "MMRegionBlocklist": [],
              "SelectionChance": "1.000000",
              "TestName": "LibraryTest",
              "CategoryRecommendationModelName": "",
              "CountryCodeAllowlist": [],
              "MMRegionAllowlist": []
            }
          ],
          "GlobalLinkCodeBlacklist": ["playlist_unvaulted_squads"],
          "SurfaceName": "CreativeDiscoverySurface_Library",
          "TestName": "",
          "primaryAssetId": "FortCreativeDiscoverySurface:CreativeDiscoverySurface_Library",
          "GlobalLinkCodeWhitelist": []
        }
      }
    }
  }
}
```
