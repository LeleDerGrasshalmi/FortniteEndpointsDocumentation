## FN Service - Storefront

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
      "name": "BRSpecialFeatured",
      "catalogEntries": []
    },
    {
      "name": "BRWeeklyStorefront",
      "catalogEntries": [
        {
          "devName": "[VIRTUAL]1 x Mi Gente for 500 MtxCurrency",
          "offerId": "v2:/01412ed4948d000bede257d1295b5e4bb454c986fa70d25842abf0b3241c9183",
          "fulfillmentIds": [],
          "dailyLimit": -1,
          "weeklyLimit": -1,
          "monthlyLimit": -1,
          "categories": [],
          "prices": [
            {
              "currencyType": "MtxCurrency",
              "currencySubType": "",
              "regularPrice": 500,
              "dynamicRegularPrice": 500,
              "finalPrice": 500,
              "saleExpiration": "9999-12-31T23:59:59.999Z",
              "basePrice": 500
            }
          ],
          "meta": {
            "NewDisplayAssetPath": "sid_placeholder_34",
            "offertag": "sparksjamloop",
            "LayoutId": "JamTracks1011.97",
            "TileSize": "Size_1_x_1",
            "AnalyticOfferGroupId": "JamTracks1011",
            "templateId": "SparksSong:sid_placeholder_34",
            "webURL": "/item-shop/jam-tracks/mi-gente-e03f6f8d",
            "inDate": "2024-08-16T00:00:00.000Z",
            "outDate": "2024-11-28T23:59:59.999Z"
          },
          "matchFilter": "",
          "filterWeight": 0.0,
          "appStoreId": [],
          "requirements": [
            {
              "requirementType": "DenyOnItemOwnership",
              "requiredId": "SparksSong:sid_placeholder_34",
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
              "value": "sid_placeholder_34"
            },
            {
              "key": "offertag",
              "value": "sparksjamloop"
            },
            {
              "key": "LayoutId",
              "value": "JamTracks1011.97"
            },
            {
              "key": "TileSize",
              "value": "Size_1_x_1"
            },
            {
              "key": "AnalyticOfferGroupId",
              "value": "JamTracks1011"
            },
            {
              "key": "templateId",
              "value": "SparksSong:sid_placeholder_34"
            },
            {
              "key": "webURL",
              "value": "/item-shop/jam-tracks/mi-gente-e03f6f8d"
            },
            {
              "key": "inDate",
              "value": "2024-08-16T00:00:00.000Z"
            },
            {
              "key": "outDate",
              "value": "2024-11-28T23:59:59.999Z"
            }
          ],
          "itemGrants": [
            {
              "templateId": "SparksSong:sid_placeholder_34",
              "quantity": 1
            }
          ],
          "additionalGrants": [],
          "sortPriority": -233,
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
              "key": "SectionID",
              "value": "LimitedTime"
            },
            {
              "key": "NewDisplayAssetPath",
              "value": "/Game/Catalog/NewDisplayAssets/S23/DAv2_RMT_ColdestCircles_QP.DAv2_RMT_ColdestCircles_QP"
            },
            {
              "key": "TileSize",
              "value": "Size_2_x_2"
            },
            {
              "key": "HideRarityBorder",
              "value": "true"
            },
            {
              "key": "ViolatorTag",
              "value": "ColdestCirclesQP"
            }
          ],
          "catalogGroup": "",
          "catalogGroupPriority": 0,
          "sortPriority": 13,
          "title": "",
          "shortDescription": "",
          "description": "",
          "displayAssetPath": "/OfferCatalog/DisplayAssets/DA_Featured_ColdestCirclesQP.DA_Featured_ColdestCirclesQP",
          "itemGrants": []
        }
      ]
    }
  ]
}
```
