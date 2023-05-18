## Fortnite - Storefront

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/storefront/v2/catalog \
Method: GET \
Auth Required: Yes (`fortnite:storefront READ`)

## Headers

`X-EpicGames-Language`: optional, response language, e.g. `de` (German)

---

_Example Response (heavily shortened)_

```json
{
  "refreshIntervalHrs": 1,
  "dailyPurchaseHrs": 24,
  "expiration": "2023-05-18T23:00:00.000Z",
  "storefronts": [
    {
      "name": "BRWeeklyStorefront",
      "catalogEntries": [
        {
          "devName": "[VIRTUAL]1 x Fishy for 300 MtxCurrency",
          "offerId": "v2:/2cccc4c4c393a0d1438f41a4d7e60bbac9cde165f37be73cee93c0827586b718",
          "fulfillmentIds": [],
          "dailyLimit": -1,
          "weeklyLimit": -1,
          "monthlyLimit": -1,
          "categories": ["Panel03"],
          "prices": [
            {
              "currencyType": "MtxCurrency",
              "currencySubType": "",
              "regularPrice": 300,
              "dynamicRegularPrice": 300,
              "finalPrice": 300,
              "saleExpiration": "9999-12-31T23:59:59.999Z",
              "basePrice": 300
            }
          ],
          "meta": {
            "NewDisplayAssetPath": "/Game/Catalog/NewDisplayAssets/DAv2_Wrap_073_TeriyakiFish2.DAv2_Wrap_073_TeriyakiFish2",
            "SectionId": "Featured2",
            "TileSize": "Small",
            "AnalyticOfferGroupId": "1"
          },
          "matchFilter": "",
          "filterWeight": 0.0,
          "appStoreId": [],
          "requirements": [
            {
              "requirementType": "DenyOnItemOwnership",
              "requiredId": "AthenaItemWrap:wrap_073_teriyakifish2",
              "minQuantity": 1
            }
          ],
          "offerType": "StaticPrice",
          "giftInfo": {
            "bIsEnabled": true,
            "forcedGiftBoxTemplateId": "",
            "purchaseRequirements": [],
            "giftRecordIds": []
          },
          "refundable": true,
          "metaInfo": [
            {
              "key": "NewDisplayAssetPath",
              "value": "/Game/Catalog/NewDisplayAssets/DAv2_Wrap_073_TeriyakiFish2.DAv2_Wrap_073_TeriyakiFish2"
            },
            {
              "key": "SectionId",
              "value": "Featured2"
            },
            {
              "key": "TileSize",
              "value": "Small"
            }
          ],
          "displayAssetPath": "/Game/Catalog/DisplayAssets/DA_Featured_Wrap_073_TeriyakiFish2.DA_Featured_Wrap_073_TeriyakiFish2",
          "itemGrants": [
            {
              "templateId": "AthenaItemWrap:wrap_073_teriyakifish2",
              "quantity": 1
            }
          ],
          "additionalGrants": [],
          "sortPriority": -9,
          "catalogGroupPriority": 0
        }
      ]
    },
    {
      "name": "BRStarterKits",
      "catalogEntries": [
        {
          "offerId": "F4FC67D34D4F0ABC742AE7826E19AB21",
          "devName": "Coldest Circles Quest Pack",
          "offerType": "StaticPrice",
          "prices": [
            {
              "currencyType": "RealMoney",
              "currencySubType": "",
              "regularPrice": 0,
              "dynamicRegularPrice": -1,
              "finalPrice": 0,
              "saleExpiration": "9999-12-31T23:59:59.999Z",
              "basePrice": 0
            }
          ],
          "categories": [],
          "dailyLimit": -1,
          "weeklyLimit": -1,
          "monthlyLimit": -1,
          "refundable": false,
          "appStoreId": [
            "",
            "bfa82be4e0f446e6a0276a5ac5caf321",
            "",
            "",
            "",
            "",
            "ICECP10000000000",
            "504c5039-3846-3043-c031-355444381c00",
            "c-seasonpack000031-ICECP1",
            "sam_ICECP1",
            "9PLPF8C15TD8",
            "ICECP10000000000"
          ],
          "requirements": [
            {
              "requirementType": "DenyOnFulfillment",
              "requiredId": "F675B1A344084379DDE5C49271E39E7B",
              "minQuantity": 1
            }
          ],
          "metaInfo": [
            {
              "key": "NewDisplayAssetPath",
              "value": "/Game/Catalog/NewDisplayAssets/S23/DAv2_RMT_ColdestCircles_QP.DAv2_RMT_ColdestCircles_QP"
            }
          ],
          "catalogGroup": "",
          "catalogGroupPriority": 0,
          "sortPriority": 19,
          "title": "Coldest Circles Quest Pack",
          "shortDescription": "",
          "description": "When fiends freeze over you get the Coldest Circles Quest Pack. Complete Quests to unlock 1 Outfit, 1 Back Bling, 1 Pickaxe and a Wrap.",
          "displayAssetPath": "/Game/Catalog/DisplayAssets/DA_Featured_ColdestCirclesQP.DA_Featured_ColdestCirclesQP",
          "itemGrants": [
            {
              "templateId": "ChallengeBundleSchedule:season24_darkice_schedule",
              "quantity": 1,
              "attributes": {}
            }
          ]
        }
      ]
    }
  ]
}
```
