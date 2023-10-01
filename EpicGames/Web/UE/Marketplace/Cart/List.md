## UE Marketplace - Cart List

URL: https://www.unrealengine.com/marketplace/api/shoppingCart \
Method: GET \
Auth Required: No

## Query Parameters

`calculatePrice`: Show price and detail (boolean)

---

_Example Response_

```json
{
  "status": "OK",
  "data": {
    "offerIds": ["1e0699cf59d64105957b4aa40f367252"],
    "totalPrice": "$25.74",
    "totalPriceDisplay": {
      "amount": "25.74",
      "symbol": "$",
      "placement": "f",
      "digits": 2
    }
  }
}
```

With calculatePrice `true`

_Example Response_

```json
{
  "status": "OK",
  "data": {
    "offers": [
      {
        "id": "1e0699cf59d64105957b4aa40f367252",
        "catalogItemId": "94db166798394a34981d3d6f427a79da",
        "namespace": "ue",
        "title": "Snapping Helper",
        "recurrence": "ONCE",
        "currencyCode": "AUD",
        "priceValue": 2574,
        "discountPriceValue": 2059,
        "voucherDiscount": 0,
        "discountPercentage": 80,
        "keyImages": [
          {
            "type": "Screenshot",
            "url": "https://cdn1.epicgames.com/ue/product/Screenshot/SHGallery07WithDescription-1920x1080-d4b550f521847456945f4f6272c790bc.jpg",
            "md5": "d4b550f521847456945f4f6272c790bc",
            "width": 1920,
            "height": 1080,
            "size": 417693,
            "uploadedDate": "2022-10-30T20:14:03.202Z"
          }
        ],
        "effectiveDate": "2021-09-05T04:43:09.636Z",
        "seller": {
          "id": "o-x8pubwykv8dsxbdwf5v6dhfb6k7pbx",
          "name": "UsefulCode"
        },
        "description": "A tool to help transform and snap actors",
        "technicalDetails": "<p>Version 1.37:</p><ul><li>Fixed Non-Unity compilation</li><li>Fixed incorrect behaivior with multiple viewports</li><li>Fixed incorrect buttons style</li></ul><p>Version 1.35:</p><ul><li>An overview of the update can be viewed in the <a href=\"https://youtu.be/R8zyYZieAdg\" rel=\"noreferrer noopener\">Demonstration</a></li><li>Added preview of selected objects. Now the result of snapping will be more visual. Can be customized or disabled in the settings</li><li>The default pivot point position can now be set via the context menu</li><li>Added distance limit beyond which vertices will not be highlighted and will not be available for selection. Can be customized or disabled in the settings</li><li>If several objects have vertices in the same place, those objects that are already selected will have priority</li></ul><p>Features:</p><ul><li>Fast and easy to learn</li><li>Highlights vertices on a geometric mesh</li><li>Temporary change of pivot point in one click</li><li>Support for all types of transformation at a temporary pivot point</li><li>Snapping actors from vertex to vertex in one click</li><li>Creation of duplicate actors with snapping in one click</li><li>In 2D snapping mode pull on one of the axes is ignored</li><li>Adapts well to different screen resolutions and DPI scale</li><li>Does not degrade editor performance. All work is done asynchronously on the background threads</li><li>Customization of the user interface</li><li>Work with static mesh and skeletal mesh components</li></ul><p>Code Modules:</p><ul><li>SnappingHelper. Editor</li></ul><p>Number of C++ Classes: 13</p><p>Network Replicated: Not used</p><p>Supported Development Platforms: Windows 32/64</p><p>Supported Target Build Platforms: Not included in the build</p>",
        "longDescription": "<p><a href=\"https://youtu.be/9qBDd7hApHA\" rel=\"noreferrer noopener\">Demonstration</a></p><p><a href=\"https://drive.google.com/file/d/1VkSfInnGTqfA9jQlK-CyMLGCf2Ig2UM8/view\" rel=\"noreferrer noopener\">Documentation</a></p><p><a href=\"https://forums.unrealengine.com/t/snapping-helper-plugin/250438\" rel=\"noreferrer noopener\">Forum page</a></p><p><br /></p><p>The tool allows you to quickly change the pivot point of the selected actor (s) and use all types of transformations. All vertices around the mouse cursor on the supported geometry will be highlighted. In one click, you can pull actors to each other, or create a duplicate and pull it.</p>",
        "isFeatured": true,
        "isCatalogItem": false,
        "categories": [
          {
            "path": "assets/codeplugins",
            "name": "Code Plugins"
          }
        ],
        "bundle": false,
        "releaseInfo": [
          {
            "id": "e8f1472d8dca4c19a870f55d8e13a347",
            "appId": "SnappingHelper_4.25",
            "compatibleApps": ["UE_4.25"],
            "platform": ["Windows", "Win32"],
            "dateAdded": "2021-08-30T00:00:00.000Z",
            "versionTitle": "v1.32_4.25"
          }
        ],
        "platforms": [
          {
            "key": "windows",
            "value": "Windows 64-bit"
          }
        ],
        "compatibleApps": ["4.25", "4.26", "4.27", "5.0", "5.1", "5.2"],
        "urlSlug": "snapping-helper",
        "purchaseLimit": 1,
        "tax": 0,
        "tags": [7776],
        "commentRatingId": "94db166798394a34981d3d6f427a79da",
        "ratingId": "1e0699cf59d64105957b4aa40f367252",
        "klass": "featured",
        "isNew": false,
        "free": false,
        "discounted": true,
        "featured": "https://cdn1.epicgames.com/ue/product/Featured/Snappinghelper_featured-894x488-e5b93a55bece0ee29005ee434b123af3.png",
        "thumbnail": "https://cdn1.epicgames.com/ue/product/Thumbnail/Snappinghelper_thumb-284x284-d019e1326bdc162012d867edc8bf1ccf.png",
        "learnThumbnail": "https://cdn1.epicgames.com/ue/product/Featured/Snappinghelper_featured-894x488-e5b93a55bece0ee29005ee434b123af3.png",
        "headerImage": "https://cdn1.epicgames.com/ue/product/Screenshot/SHGallery07WithDescription-1920x1080-d4b550f521847456945f4f6272c790bc.jpg",
        "status": "ACTIVE",
        "price": "$25.74",
        "discount": "$5.15",
        "discountPrice": "$20.59",
        "ownedCount": 0,
        "canPurchase": true,
        "owned": false
      }
    ],
    "offerIds": ["1e0699cf59d64105957b4aa40f367252"],
    "totalPrice": "$25.74",
    "totalAmount": 2574,
    "totalCouponDiscount": "$0.00",
    "totalDiscountPrice": "$20.59",
    "appliedCoupon": false
  }
}
```
