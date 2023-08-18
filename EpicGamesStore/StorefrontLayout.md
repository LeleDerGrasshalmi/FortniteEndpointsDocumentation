## Epic Games Store - Storefront Layout (GraphQL Response)

URL: https://store-site-backend-static-ipv4.ak.epicgames.com/storefrontLayout \
Method: GET \
Auth Required: No

## Query Parameters

`locale`: The requested Language, defaults to english

> All Query Params are optional and there may be more

---

_Example Response (shortened)_

```json
{
  "data": {
    "Storefront": {
      "storefrontModules": [
        {
          "id": "new-carousel-definitive",
          "type": "saleCarousel",
          "title": "New Featured Carousel ",
          "slides": [
            {
              "title": "EA SPORTS™ FC Ultimate Edition",
              "eyebrow": "Available September 29",
              "description": "Pre-purchase the Ultimate Edition by 22 Aug for a UCL or UWCL Hero.",
              "textColor": null,
              "accentColor": null,
              "textAccentColor": null,
              "theme": {
                "preferredMode": null,
                "light": {
                  "theme": null,
                  "accent": null
                },
                "dark": {
                  "theme": null,
                  "accent": null
                }
              },
              "image": {
                "src": "https://cdn2.unrealengine.com/egs-fc24-ultimate-carousel-desktop-1920x1080-24ba0952c33e.jpg",
                "altText": "Pre-Purchase EA SPORTS FC™ on Epic Games Store"
              },
              "mobileImage": {
                "src": "https://cdn2.unrealengine.com/egs-fc24-ultimate-carousel-mobile-1200x1600-0ae9bad694d2.jpg",
                "altText": "Pre-Purchase EA SPORTS FC™ on Epic Games Store"
              },
              "logoImage": {
                "src": "https://cdn2.unrealengine.com/egs-fc24-ultimate-carousel-logo-350x261-778d03f6f36d.png",
                "altText": "Pre-Purchase EA SPORTS FC™ on Epic Games Store"
              },
              "thumbnail": {
                "src": "https://cdn2.unrealengine.com/egs-fc24-ultimate-carousel-thumb-1200x1600-deff2ea75f68.jpg",
                "altText": "Pre-Purchase EA SPORTS FC™ on Epic Games Store"
              },
              "link": {
                "src": "/p/ea-sports-fc-24--ultimate-edition",
                "linkText": "Pre-Purchase Now"
              },
              "videoRecipe": null,
              "regionRestrictions": {
                "filterType": "BLACKLIST",
                "appliedCountries": "BE,RU"
              },
              "offer": {
                "namespace": "4750c68b2bfa4f43933b81cfd5cc510c",
                "id": "cfc305430d514c6887b021104d23bd55"
              }
            }
          ]
        },
        {
          "id": "blade-newtotheepicstore",
          "type": "group",
          "title": "Now On The Epic Games Store",
          "link": {
            "src": null,
            "linkText": null
          },
          "titleIcon": "NONE",
          "hideTitle": false,
          "groupStyle": "standard",
          "offerType": "topic",
          "offerPresentation": "slider",
          "cardType": "TALL",
          "offers": [
            {
              "namespace": "3376364c2a914c1fbde839f5cf8824f6",
              "id": "cf5be2c093914084881aa74cc0367ef3",
              "offer": {
                "title": "Secret Agent 001",
                "id": "cf5be2c093914084881aa74cc0367ef3",
                "namespace": "3376364c2a914c1fbde839f5cf8824f6",
                "offerType": "BASE_GAME",
                "expiryDate": null,
                "status": "ACTIVE",
                "isCodeRedemptionOnly": false,
                "description": "Welcome to another mission Mr. Agent 001. Are you ready for a new theft?",
                "effectiveDate": "2023-07-29T07:00:00.000Z",
                "viewableDate": "2023-07-12T07:00:00.000Z",
                "pcReleaseDate": "2022-12-02T08:00:00.000Z",
                "releaseDate": "2023-07-29T07:00:00.000Z",
                "approximateReleasePlan": null,
                "prePurchase": null,
                "keyImages": [
                  {
                    "type": "Thumbnail",
                    "url": "https://cdn1.epicgames.com/spt-assets/471a0f14344549cfaa455f8f14bf0951/secret-agent-001-5neyp.jpg"
                  }
                ],
                "seller": {
                  "id": "o-zejr7w3wpnqtvlbug6r56mn53csnwj",
                  "name": "Atomic Fabrik"
                },
                "productSlug": null,
                "urlSlug": "f1c59d35762245d7bffdf93f5f3f9063",
                "items": [
                  {
                    "id": "56c359777fd64c84aa5787a30a65e7d1",
                    "namespace": "3376364c2a914c1fbde839f5cf8824f6"
                  }
                ],
                "customAttributes": [
                  {
                    "key": "isBlockchainUsed",
                    "value": "false"
                  }
                ],
                "developerDisplayName": "Atomic Fabrik",
                "publisherDisplayName": "Atomic Fabrik",
                "categories": [
                  {
                    "path": "games"
                  }
                ],
                "catalogNs": {
                  "mappings": [
                    {
                      "pageSlug": "obelixes-tower-defense-0efb67",
                      "pageType": "productHome"
                    }
                  ]
                },
                "offerMappings": [
                  {
                    "pageSlug": "obelixes-tower-defense-0efb67",
                    "pageType": "productHome"
                  }
                ],
                "price": {
                  "totalPrice": {
                    "discountPrice": 199,
                    "originalPrice": 199,
                    "voucherDiscount": 0,
                    "discount": 0,
                    "fmtPrice": {
                      "originalPrice": "$1.99",
                      "discountPrice": "$1.99",
                      "intermediatePrice": "$1.99"
                    },
                    "currencyCode": "USD",
                    "currencyInfo": {
                      "decimals": 2,
                      "symbol": "$"
                    }
                  },
                  "lineOffers": [
                    {
                      "appliedRules": []
                    }
                  ]
                },
                "linkedOfferId": null,
                "linkedOffer": null,
                "countriesBlacklist": ["KR"],
                "countriesWhitelist": null
              }
            }
          ]
        },
        {
          "id": "module-breaker-footer",
          "type": "subModules",
          "title": "",
          "modules": [
            {
              "id": "module-content/breaker-free-games-evergreen",
              "type": "breaker",
              "title": "Free Games",
              "titleGroup": " Free Games",
              "description": "Explore free and free-to-play games from our collection. Come back every Thursday for a new free game!",
              "backgroundColors": null,
              "layout": "singleImage",
              "action": "link",
              "couponSlug": null,
              "eyebrow": null,
              "videoRecipe": null,
              "link": {
                "src": "/free-games",
                "linkText": "Play Now"
              },
              "image": {
                "src": "https://cdn2.unrealengine.com/egs-free-games-breaker-may-2023-1920x1080-3d7b336fd40c.jpg",
                "alt": "Browse Free titles on Epic Games"
              },
              "regionRestrictions": {
                "filterType": "NONE",
                "appliedCountries": ""
              },
              "offer": {
                "namespace": "",
                "id": ""
              }
            }
          ]
        }
      ]
    }
  },
  "extensions": {}
}
```
