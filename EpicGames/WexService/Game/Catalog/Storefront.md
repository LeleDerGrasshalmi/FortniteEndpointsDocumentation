## Wex Service - Catalog: Storefront

URL: https://wex-public-service-live-prod.ol.epicgames.com/wex/api/storefront/v2/catalog \
Method: GET \
Auth Required: Yes (`wexp:storefront READ`)

---

_Example Response (shortened)_

```json
{
  "refreshIntervalHrs": 12,
  "dailyPurchaseHrs": 12,
  "expiration": "2022-11-11T00:00:00.000Z",
  "storefronts": [
    {
      "name": "SecretShopPage3",
      "catalogEntries": [
        {
          "offerId": "3130D8B1A91C415AAB8FDB40A039ED36",
          "devName": "SecretShop.Page03.UnderworldTrader.50",
          "offerType": "StaticPrice",
          "prices": [
            {
              "currencyType": "MtxCurrency",
              "currencySubType": "",
              "regularPrice": 200,
              "dynamicRegularPrice": -1,
              "finalPrice": 140,
              "saleType": "AmountOff",
              "saleExpiration": "9999-12-31T23:59:59.999Z",
              "basePrice": 140
            }
          ],
          "categories": [],
          "dailyLimit": 1,
          "weeklyLimit": -1,
          "monthlyLimit": -1,
          "refundable": false,
          "appStoreId": ["", "", "", "", "", "", "", "", "", ""],
          "requirements": [],
          "metaInfo": [
            {
              "key": "VipLevelMin",
              "value": "3"
            }
          ],
          "catalogGroup": "",
          "catalogGroupPriority": 0,
          "sortPriority": 0,
          "title": "",
          "shortDescription": "",
          "description": "",
          "displayAssetPath": "",
          "itemGrants": [
            {
              "templateId": "Reagent:Reagent_Shard_Water",
              "quantity": 1
            }
          ]
        }
      ]
    }
  ]
}
```
