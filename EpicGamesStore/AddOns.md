## Epic Games Store - Add-Ons

URL: https://www.epicgames.com/graphql \
Method: POST \
Auth Required: No

## Body
```json
{
    "query":"query searchStoreQuery($allowCountries: String, $category: String, $count: Int, $country: String!, $keywords: String, $locale: String, $namespace: String, $itemNs: String, $sortBy: String, $sortDir: String, $start: Int, $tag: String, $releaseDate: String, $withPrice: Boolean = false, $withPromotions: Boolean = false, $priceRange: String, $freeGame: Boolean, $onSale: Boolean, $effectiveDate: String) {\n  Catalog {\n    searchStore(\n      allowCountries: $allowCountries\n      category: $category\n      count: $count\n      country: $country\n      keywords: $keywords\n      locale: $locale\n      namespace: $namespace\n      itemNs: $itemNs\n      sortBy: $sortBy\n      sortDir: $sortDir\n      releaseDate: $releaseDate\n      start: $start\n      tag: $tag\n      priceRange: $priceRange\n      freeGame: $freeGame\n      onSale: $onSale\n      effectiveDate: $effectiveDate\n    ) {\n      elements {\n       id\n        namespace\n      title\n      title4Sort\n                description\n       creationDate\n        viewableDate\n        releaseDate\n        pcReleaseDate\n        effectiveDate\n        expiryDate\n        lastModifiedDate\n        keyImages {\n          type\n          url\n          size\n          width\n          height\n          uploadedDate\n       }\n        seller {\n          id\n          name\n        }\n        productSlug\n          urlSlug\n        url\n        tags {\n          id\n        }\n        items {\n          id\n          namespace\n        }\n        customAttributes {\n          key\n          value\n        }\n        categories {\n          path\n        }\n        catalogNs {\n          mappings(pageType: \"productHome\") {\n            pageSlug\n            pageType\n          }\n        }\n        offerMappings {\n          pageSlug\n          pageType\n        }\n        developerDisplayName\n        publisherDisplayName\n        currentPrice\n        basePrice\n        price(country: $country) @include(if: $withPrice) {\n          totalPrice {\n            discountPrice\n            originalPrice\n            voucherDiscount\n            discount\n            currencyCode\n            currencyInfo {\n              decimals\n            }\n            fmtPrice(locale: $locale) {\n              originalPrice\n              discountPrice\n              intermediatePrice\n            }\n          }\n          lineOffers {\n            appliedRules {\n              id\n              endDate\n              discountSetting {\n                discountType\n              }\n            }\n          }\n        }\n        promotions(category: $category) @include(if: $withPromotions) {\n          promotionalOffers {\n            promotionalOffers {\n              startDate\n              endDate\n              discountSetting {\n                discountType\n                discountPercentage\n              }\n            }\n          }\n          upcomingPromotionalOffers {\n            promotionalOffers {\n              startDate\n              endDate\n              discountSetting {\n                discountType\n                discountPercentage\n              }\n            }\n          }\n        }\n      }\n      paging {\n        count\n        total\n      }\n    }\n  }\n}\n",
   "variables":{
      "category":"digitalextras/book|addons|digitalextras/soundtrack|digitalextras/video",
      "count": 100,
      "country":"US",
      "keywords":"",
      "locale":"en",
      "namespace":"fn",
      "sortBy":"releaseDate",
      "sortDir":"DESC",
      "allowCountries":"US",
      "start":0,
      "tag":"",
      "releaseDate":"[,{CurrentIsoDateString}]",
      "withPrice":true
   }
}
```
