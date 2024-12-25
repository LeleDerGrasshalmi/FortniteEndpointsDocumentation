## FN EOS Inventory Service: Player Inventory

URL: https://fngw-svc-ds-livefn.ol.epicgames.com/api/inventory/v3/:deploymentId/players/:productUserId/:inventoryName \
Method: GET \
Auth Required: Yes (`inventories:readPlayerInventoryForLocalUser`)

## Path Parameters

`deploymentId`: The Deployment Id from env configuration, for `live-fn` it is `62a9473a2dca46b29ccf17577fcf42d7` <br/>
`productUserId`: Your EOS Connect Product User Id <br/>
`inventoryName`: The inventory name, _must be URL Encoded_, currently only `/br` is known

---

_Example Response (played s30)_

```json
{
  "binary": null,
  "inventory": {
    "playerId": "0002e2257ef14f2889c6cb3d079d3141",
    "inventoryName": "/br",
    "prefix": "/",
    "instance": "00000000-0000-0000-0000-000000000000",
    "contents": {
      "/accoladecollection30": "{\\\"pfwaccoladecollection_module\\\":{\\\"fortcontrollercomponent_accoladecollection\\\":{\\\"version\\\":{\\\"guid\\\":\\\"9F878C14-F88B-45BC-8275-913E43B37144\\\",\\\"version\\\":0},\\\"data\\\":{\\\"accoladecollection_achievedaccolades\\\":{\\\"version\\\":{\\\"guid\\\":\\\"CA088ECC-E46D-492B-A12D-CCFD3FE9EF4A\\\",\\\"version\\\":0},\\\"data\\\":{\\\"accoladecollection_achievedaccolades_0\\\":{\\\"accoladeName\\\":\\\"Accolade_Survival_SurvivorOne\\\",\\\"accoladeCount\\\":16},\\\"accoladecollection_achievedaccolades_1\\\":{\\\"accoladeName\\\":\\\"Accolade_Resources_AmmoScrounger\\\",\\\"accoladeCount\\\":6},\\\"accoladecollection_achievedaccolades_2\\\":{\\\"accoladeName\\\":\\\"Accolade_Seasonal_SugarBomb\\\",\\\"accoladeCount\\\":10},\\\"accoladecollection_achievedaccolades_3\\\":{\\\"accoladeName\\\":\\\"Accolade_Survival_SurvivorTwo\\\",\\\"accoladeCount\\\":16},\\\"accoladecollection_achievedaccolades_4\\\":{\\\"accoladeName\\\":\\\"Accolade_Resources_LootCollector\\\",\\\"accoladeCount\\\":8},\\\"accoladecollection_achievedaccolades_5\\\":{\\\"accoladeName\\\":\\\"Accolade_Resources_AmmoScavenger\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_6\\\":{\\\"accoladeName\\\":\\\"Accolade_Resources_DemolitionSpecialist\\\",\\\"accoladeCount\\\":11},\\\"accoladecollection_achievedaccolades_7\\\":{\\\"accoladeName\\\":\\\"Accolade_Resources_DemolitionExpert\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_8\\\":{\\\"accoladeName\\\":\\\"Accolade_Seasonal_DemolitionDerby\\\",\\\"accoladeCount\\\":6},\\\"accoladecollection_achievedaccolades_9\\\":{\\\"accoladeName\\\":\\\"Accolade_Seasonal_RoadTrip\\\",\\\"accoladeCount\\\":9},\\\"accoladecollection_achievedaccolades_10\\\":{\\\"accoladeName\\\":\\\"Accolade_Survival_SurvivorThree\\\",\\\"accoladeCount\\\":4},\\\"accoladecollection_achievedaccolades_11\\\":{\\\"accoladeName\\\":\\\"Accolade_Seasonal_HotRod\\\",\\\"accoladeCount\\\":7},\\\"accoladecollection_achievedaccolades_12\\\":{\\\"accoladeName\\\":\\\"Accolade_Resources_DemolitionMaster\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_13\\\":{\\\"accoladeName\\\":\\\"Accolade_Special_BetterLateThanNever\\\",\\\"accoladeCount\\\":12},\\\"accoladecollection_achievedaccolades_14\\\":{\\\"accoladeName\\\":\\\"Accolade_Combat_DoubleElimination\\\",\\\"accoladeCount\\\":10},\\\"accoladecollection_achievedaccolades_15\\\":{\\\"accoladeName\\\":\\\"Accolade_FirstInMatch_FastTalker\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_16\\\":{\\\"accoladeName\\\":\\\"Accolade_Combat_SpeedBump\\\",\\\"accoladeCount\\\":7},\\\"accoladecollection_achievedaccolades_17\\\":{\\\"accoladeName\\\":\\\"Accolade_Combat_SingleDigit\\\",\\\"accoladeCount\\\":12},\\\"accoladecollection_achievedaccolades_18\\\":{\\\"accoladeName\\\":\\\"Accolade_Survival_Medical_Specialist\\\",\\\"accoladeCount\\\":12},\\\"accoladecollection_achievedaccolades_19\\\":{\\\"accoladeName\\\":\\\"Accolade_Weapons_MistOfMetal\\\",\\\"accoladeCount\\\":6},\\\"accoladecollection_achievedaccolades_20\\\":{\\\"accoladeName\\\":\\\"Accolade_Combat_AntiAirPersonnel\\\",\\\"accoladeCount\\\":6},\\\"accoladecollection_achievedaccolades_21\\\":{\\\"accoladeName\\\":\\\"Accolade_Weapons_RainingLead\\\",\\\"accoladeCount\\\":4},\\\"accoladecollection_achievedaccolades_22\\\":{\\\"accoladeName\\\":\\\"Accolade_Survival_Medical_Expert\\\",\\\"accoladeCount\\\":7},\\\"accoladecollection_achievedaccolades_23\\\":{\\\"accoladeName\\\":\\\"Accolade_Survival_Medical_Master\\\",\\\"accoladeCount\\\":6},\\\"accoladecollection_achievedaccolades_24\\\":{\\\"accoladeName\\\":\\\"Accolade_FirstInMatch_AmmoAce\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_25\\\":{\\\"accoladeName\\\":\\\"Accolade_Survival_Shield_Specialist\\\",\\\"accoladeCount\\\":2},\\\"accoladecollection_achievedaccolades_26\\\":{\\\"accoladeName\\\":\\\"Accolade_Resources_GoldRush\\\",\\\"accoladeCount\\\":3},\\\"accoladecollection_achievedaccolades_27\\\":{\\\"accoladeName\\\":\\\"Accolade_Resources_GildedGlory\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_28\\\":{\\\"accoladeName\\\":\\\"Accolade_Special_WeaponSmuggler\\\",\\\"accoladeCount\\\":3},\\\"accoladecollection_achievedaccolades_29\\\":{\\\"accoladeName\\\":\\\"Accolade_Combat_FirstToTheFeast\\\",\\\"accoladeCount\\\":9},\\\"accoladecollection_achievedaccolades_30\\\":{\\\"accoladeName\\\":\\\"Accolade_Combat_DoubleDigits\\\",\\\"accoladeCount\\\":7},\\\"accoladecollection_achievedaccolades_31\\\":{\\\"accoladeName\\\":\\\"Accolade_Weapons_Melee_Specialist\\\",\\\"accoladeCount\\\":4},\\\"accoladecollection_achievedaccolades_32\\\":{\\\"accoladeName\\\":\\\"Accolade_Survival_LightBreeze\\\",\\\"accoladeCount\\\":8},\\\"accoladecollection_achievedaccolades_33\\\":{\\\"accoladeName\\\":\\\"Accolade_Weapons_SMG_Specialist\\\",\\\"accoladeCount\\\":2},\\\"accoladecollection_achievedaccolades_34\\\":{\\\"accoladeName\\\":\\\"Accolade_Combat_Headshot\\\",\\\"accoladeCount\\\":8},\\\"accoladecollection_achievedaccolades_35\\\":{\\\"accoladeName\\\":\\\"Accolade_Weapons_Shotgun_Specialist\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_36\\\":{\\\"accoladeName\\\":\\\"Accolade_Survival_BarelyRaining\\\",\\\"accoladeCount\\\":4},\\\"accoladecollection_achievedaccolades_37\\\":{\\\"accoladeName\\\":\\\"Accolade_Weapons_HighCaliberHail\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_38\\\":{\\\"accoladeName\\\":\\\"Accolade_Seasonal_RoadRage\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_39\\\":{\\\"accoladeName\\\":\\\"Accolade_FirstInMatch_GearHead\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_40\\\":{\\\"accoladeName\\\":\\\"Accolade_FirstInMatch_EarlyBird\\\",\\\"accoladeCount\\\":2},\\\"accoladecollection_achievedaccolades_41\\\":{\\\"accoladeName\\\":\\\"Accolade_Special_StillGotEm\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_42\\\":{\\\"accoladeName\\\":\\\"Accolade_Resources_BottomlessClip\\\",\\\"accoladeCount\\\":3},\\\"accoladecollection_achievedaccolades_43\\\":{\\\"accoladeName\\\":\\\"Accolade_Combat_ImpossibleShot\\\",\\\"accoladeCount\\\":2},\\\"accoladecollection_achievedaccolades_44\\\":{\\\"accoladeName\\\":\\\"Accolade_Weapons_AndTheKitchenSink\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_45\\\":{\\\"accoladeName\\\":\\\"Accolade_Combat_MultiElimination\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_46\\\":{\\\"accoladeName\\\":\\\"Accolade_Combat_EliminationCollector\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_47\\\":{\\\"accoladeName\\\":\\\"Accolade_Weapons_Melee_Expert\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_48\\\":{\\\"accoladeName\\\":\\\"Accolade_Seasonal_GauntletBarrage\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_49\\\":{\\\"accoladeName\\\":\\\"Accolade_Special_FruitsAndVeggies\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_50\\\":{\\\"accoladeName\\\":\\\"Accolade_Survival_ActuallyUseBandages\\\",\\\"accoladeCount\\\":2},\\\"accoladecollection_achievedaccolades_51\\\":{\\\"accoladeName\\\":\\\"Accolade_Combat_DistanceShot\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_52\\\":{\\\"accoladeName\\\":\\\"Accolade_Resources_LootStockpiler\\\",\\\"accoladeCount\\\":2},\\\"accoladecollection_achievedaccolades_53\\\":{\\\"accoladeName\\\":\\\"Accolade_Resources_Resourcefulness\\\",\\\"accoladeCount\\\":2},\\\"accoladecollection_achievedaccolades_54\\\":{\\\"accoladeName\\\":\\\"Accolade_Survival_BattenTheHatches\\\",\\\"accoladeCount\\\":1},\\\"accoladecollection_achievedaccolades_55\\\":{\\\"accoladeName\\\":\\\"Accolade_Combat_LongShot\\\",\\\"accoladeCount\\\":1}}},\\\"accoladecollection_pinnedaccolade\\\":{\\\"version\\\":{\\\"guid\\\":\\\"3F935CB3-BE87-4AB5-999C-655DCB378F9A\\\",\\\"version\\\":0},\\\"data\\\":{\\\"accoladeName\\\":\\\"None\\\"}},\\\"accoladecollection_unacknowledgedaccolades\\\":{\\\"version\\\":{\\\"guid\\\":\\\"7C75E700-CB8B-47F2-997A-A24411FEEDBD\\\",\\\"version\\\":0},\\\"data\\\":{\\\"accoladeNames\\\":[]}}}}}}",
      "/accoladecollection30.meta": "{\\\"version\\\":1,\\\"serializer\\\":\\\"JsonObjectAsSingleString\\\"}"
    }
  },
  "continuationToken": null
}
```

_Example Response (didnt play s30)_

```json
{
  "binary": null,
  "inventory": {
    "playerId": "0002e2257ef14f2889c6cb3d079d3141",
    "inventoryName": "/br",
    "prefix": "/",
    "instance": "00000000-0000-0000-0000-000000000000",
    "contents": {
      "/accoladecollection30": "{\\\"pfwaccoladecollection_module\\\":{}}",
      "/accoladecollection30.meta": "{\\\"version\\\":1,\\\"serializer\\\":\\\"JsonObjectAsSingleString\\\"}"
    }
  },
  "continuationToken": null
}
```

> `instance` has been redacted
