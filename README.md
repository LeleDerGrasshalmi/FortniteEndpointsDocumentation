# Fortnite Related Endpont Documentation
By jemcer#1009 &amp; LeleDerGrasshalm#1872

## Epic Games Store

| Name | URL | Method | Auth Required | Body
| ----------- | ----------- | ----------- | ----------- | ----------- |
| Site | https://store-content.ak.epicgames.com/api/en-US/content/products/fortnite | GET | No | None|
| Add Ons | https://www.epicgames.com/graphql | POST | No | {"query": "query searchStoreQuery($allowCountries: String, $category: String, $count: Int, $country: String!, $keywords: String, $locale: String, $namespace: String, $itemNs: String, $sortBy: String, $sortDir: String, $start: Int, $tag: String, $releaseDate: String, $withPrice: Boolean = false, $withPromotions: Boolean = false, $priceRange: String, $freeGame: Boolean, $onSale: Boolean, $effectiveDate: String) {\n  Catalog {\n    searchStore(\n      allowCountries: $allowCountries\n      category: $category\n      count: $count\n      country: $country\n      keywords: $keywords\n      locale: $locale\n      namespace: $namespace\n      itemNs: $itemNs\n      sortBy: $sortBy\n      sortDir: $sortDir\n      releaseDate: $releaseDate\n      start: $start\n      tag: $tag\n      priceRange: $priceRange\n      freeGame: $freeGame\n      onSale: $onSale\n      effectiveDate: $effectiveDate\n    ) {\n      elements {\n        title\n        id\n        namespace\n        description\n        effectiveDate\n        keyImages {\n          type\n          url\n        }\n        currentPrice\n        seller {\n          id\n          name\n        }\n        productSlug\n        urlSlug\n        url\n        tags {\n          id\n        }\n        items {\n          id\n          namespace\n        }\n        customAttributes {\n          key\n          value\n        }\n        categories {\n          path\n        }\n        catalogNs {\n          mappings(pageType: \"productHome\") {\n            pageSlug\n            pageType\n          }\n        }\n        offerMappings {\n          pageSlug\n          pageType\n        }\n        developerDisplayName\n        publisherDisplayName\n        price(country: $country) @include(if: $withPrice) {\n          totalPrice {\n            discountPrice\n            originalPrice\n            voucherDiscount\n            discount\n            currencyCode\n            currencyInfo {\n              decimals\n            }\n            fmtPrice(locale: $locale) {\n              originalPrice\n              discountPrice\n              intermediatePrice\n            }\n          }\n          lineOffers {\n            appliedRules {\n              id\n              endDate\n              discountSetting {\n                discountType\n              }\n            }\n          }\n        }\n        promotions(category: $category) @include(if: $withPromotions) {\n          promotionalOffers {\n            promotionalOffers {\n              startDate\n              endDate\n              discountSetting {\n                discountType\n                discountPercentage\n              }\n            }\n          }\n          upcomingPromotionalOffers {\n            promotionalOffers {\n              startDate\n              endDate\n              discountSetting {\n                discountType\n                discountPercentage\n              }\n            }\n          }\n        }\n      }\n      paging {\n        count\n        total\n      }\n    }\n  }\n}\n","variables": {
         "category": "digitalextras/book|addons|digitalextras/soundtrack|digitalextras/video",
         "count": 40,
         "country": "DE",
         "keywords": "",
         "locale": "de",
         "namespace": "fn",
         "sortBy": "releaseDate",
         "sortDir": "DESC",
         "allowCountries": "DE",
         "start": 0,
         "tag": "",
         "releaseDate": "[,2021-09-27T14:17:58.778Z]",
         "withPrice": true
      }
   }

## Fortnite Website

| Name | URL | Method | Auth Required | Body
| ----------- | ----------- | ----------- | ----------- | ----------- |
| Competetive Calendar | https://www.epicgames.com/fortnite/competitive/api/en/calendar | POST | No | {}
| Competetive Events | https://www.epicgames.com/fortnite/competitive/api/en/events | GET | No | None
| Cosplay | https://www.epicgames.com/fortnite/en/api/cosplay | GET | No | None
| Creative Featured Islands | https://www.epicgames.com/fortnite/api/creative/featured-islands | GET | No | None
| Help Center | https://www.epicgames.com/fortnite/en/api/help-center | GET | No | None
| StW Founder Packs | https://www.epicgames.com/fortnite/api/founders-packs | GET | No | None
| Subscription | https://www.epicgames.com/fortnite/api/subscription-offer | GET | No | None

## Fortnite

| Name | URL | Method | Auth Required | Body
| ----------- | ----------- | ----------- | ----------- | ----------- |
| Content | https://fortnitecontent-website-prod07.ol.epicgames.com/content/api/pages/fortnite-game | GET | No | None
| Calendar/Timeline | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/calendar/v1/timeline | GET | YES | None
| Keychain | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/storefront/v2/keychain | GET | YES | None
| Catalog/Store | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/storefront/v2/catalog | GET | YES | None
| Info for AppstoreId(s) | https://catalog-public-service-prod06.ol.epicgames.com/catalog/api/shared/bulk/offers?id={AppstoreId} | GET | YES | None
| Server Status | https://lightswitch-public-service-prod06.ol.epicgames.com/lightswitch/api/service/bulk/status?serviceId=Fortnite | GET | YES | None
| Manifest - Windows | https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/v2/platform/Windows/namespace/fn/catalogItem/4fe75bbc5a674f4f9b356b5c90567da5/app/Fortnite/label/Live | GET | YES | None
| Manifest - Android | https://launcher-public-service-prod-m.ol.epicgames.com/launcher/api/public/assets/Android/5cb97847cee34581afdbc445400e2f77/FortniteContentBuilds?label=Live | GET | YES | None
| Manifest - IOS | https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/IOS/5cb97847cee34581afdbc445400e2f77/FortniteContentBuilds?label=Live | GET | YES | None
