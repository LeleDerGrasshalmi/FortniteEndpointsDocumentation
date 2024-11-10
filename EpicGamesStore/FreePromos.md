## Epic Games Store - Free Promos (GraphQL Response)

URL: https://store-site-backend-static-ipv4.ak.epicgames.com/freeGamesPromotions \
Method: GET \
Auth Required: No

## Query Parameters

`locale`: The requested Language, defaults to english <br/>
`country`: Determines the price and which currency is shown<br/>
`allowCountries`: Show all promos available in the requested Countries

> All Query Params are optional and there may be more

---

_Example Response (shortened)_

```json
{
  "data": {
    "Catalog": {
      "searchStore": {
        "elements": [
          {
            "title": "Black Book",
            "id": "0bce0871129140d894da3789e2fe0a7f",
            "namespace": "8211dc6089af4542926b7a8137b9079e",
            "description": "Spiele eine junge Zauberin in „Black Book“, einem düsteren RPG-Abenteuer, das auf slawischen Mythen beruht. Kämpfe gegen dunkle Mächte und erkunde eine Welt, in der Menschen und mythologische Wesen leben.",
            "effectiveDate": "2021-08-10T17:00:00.000Z",
            "offerType": "BASE_GAME",
            "expiryDate": null,
            "viewableDate": "2021-08-10T17:00:00.000Z",
            "status": "ACTIVE",
            "isCodeRedemptionOnly": false,
            "keyImages": [
              {
                "type": "Thumbnail",
                "url": "https://cdn1.epicgames.com/salesEvent/salesEvent/EGS_BlackBook_Morteshka_S2_1200x1600-1202bf8f0d59ae480ba82d1850dc6eaa"
              }
            ],
            "seller": {
              "id": "o-p9883lvrpllhyd7sad6tgxv53mdyh5",
              "name": "Hypetrain Digital"
            },
            "productSlug": "black-book",
            "urlSlug": "tommes-general-audience",
            "url": null,
            "items": [
              {
                "id": "d0c6ec2f180e4b34b1202f12fe489acf",
                "namespace": "8211dc6089af4542926b7a8137b9079e"
              }
            ],
            "customAttributes": [
              {
                "key": "com.epicgames.app.productSlug",
                "value": "black-book"
              }
            ],
            "categories": [
              {
                "path": "freegames"
              }
            ],
            "tags": [
              {
                "id": "22737"
              }
            ],
            "catalogNs": {
              "mappings": [
                {
                  "pageSlug": "black-book",
                  "pageType": "productHome"
                }
              ]
            },
            "offerMappings": [],
            "price": {
              "totalPrice": {
                "discountPrice": 0,
                "originalPrice": 2499,
                "voucherDiscount": 0,
                "discount": 2499,
                "currencyCode": "USD",
                "currencyInfo": {
                  "decimals": 2
                },
                "fmtPrice": {
                  "originalPrice": "24,99 $",
                  "discountPrice": "0",
                  "intermediatePrice": "0"
                }
              },
              "lineOffers": [
                {
                  "appliedRules": [
                    {
                      "id": "b3485196083843718efaed71b6be3abf",
                      "endDate": "2023-08-24T15:00:00.000Z",
                      "discountSetting": {
                        "discountType": "PERCENTAGE"
                      }
                    }
                  ]
                }
              ]
            },
            "promotions": {
              "promotionalOffers": [
                {
                  "promotionalOffers": [
                    {
                      "startDate": "2023-08-17T15:00:00.000Z",
                      "endDate": "2023-08-24T15:00:00.000Z",
                      "discountSetting": {
                        "discountType": "PERCENTAGE",
                        "discountPercentage": 0
                      }
                    }
                  ]
                }
              ],
              "upcomingPromotionalOffers": []
            }
          }
        ],
        "paging": {
          "count": 1000,
          "total": 5
        }
      }
    }
  },
  "extensions": {}
}
```
