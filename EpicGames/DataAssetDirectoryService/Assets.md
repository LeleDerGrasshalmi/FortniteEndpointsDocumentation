## DAD Service - Assets (Gamefile Overwrites)

URL: https://data-asset-directory-public-service-prod.ol.epicgames.com/api/v1/assets/:gameId/:branch/:changelist \
Method: POST \
Auth Required: Yes (`dad:{gameId}:assets:* READ`)

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

`gameId`: `Fortnite` (Lowercased for the Permission) <br/>
`branch`: The Build Branch, e.g. `++Fortnite+Release-26.10` <br/>
`changelist`: The Version Changelist, e.g. `27681420`

## Query Parameters

`appId`: `Fortnite`

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
