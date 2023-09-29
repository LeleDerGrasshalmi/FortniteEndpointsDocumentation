## UE Marketplace - Seller Info

URL: https://www.unrealengine.com/marketplace/api/assets/seller/:username \
Method: GET \
Auth Required: No

### Path Parameters

`username`: Username of seller

---

_Example Response_

```json
{
  "status": "OK",
  "data": {
    "elements": [
      {
        "id": "dca36a5516154449bcc07b25834a1e00",
        "catalogItemId": "aab9066e3e644652873d24900f8dd84f",
        "namespace": "ue",
        "title": "Cropout Sample Project",
        "recurrence": "ONCE",
        "currencyCode": "AUD",
        "priceValue": 0,
        "keyImages": [
          {
            "type": "Featured",
            "url": "https://cdn1.epicgames.com/item/ue/Featured_894x488-c65b7da2d8757ec48bf68806a3322e62",
            "md5": "c65b7da2d8757ec48bf68806a3322e62",
            "width": 894,
            "height": 488,
            "size": 155755,
            "uploadedDate": "2023-06-26T18:53:58.584Z"
          }
        ],
        "viewableDate": "2023-07-27T05:00:00.000Z",
        "effectiveDate": "2023-07-27T09:00:00.000Z",
        "seller": {
          "id": "o-aa83a0a9bc45e98c80c1b1c9d92e9e",
          "noAi": false,
          "owner": "311cffd7000046919e47765426990332",
          "status": "ACTIVE",
          "accepted": [
            {
              "ns": "ue",
              "custom": false
            }
          ],
          "financeCheckExempted": true,
          "name": "Epic Games",
          "supportEmail": "marketplace-support@unrealengine.com"
        },
        "description": "Cropout is a Casual RTS game sample that shows you best practices for creating a cross-platform project in UE5.",
        "technicalDetails": "[\n    { \n        \"Image\": \"download\", \n        \"Text\": \"Download Sample\"\n    }\n]",
        "longDescription": "<p>Cropout is a sample top-down Casual RTS game that demonstrates all the best practices for building a project designed for cross-platform release. From low-spec mobile devices to powerful gaming consoles and PCs, Cropout is set up to build once and then distribute everywhere. Cropout also demonstrates new engine features like Common UI, Enhanced Input, and Geometry Script.</p> <p>With a family-friendly farming style, Cropout is suitable for beginners, educators, and anyone wanting to learn to create this genre of gameplay. </p> <p>You will be able to spend hours digging into all the Blueprints, materials, VFX, characters, and more. We hope you enjoy!</p> <p>For more information and helpful resources, visit <a href=\"https://unrealengine.com/cropout\" rel=\"noreferrer noopener\">unrealengine.com/cropout</a>.</p>\n<b>UE-Only Content</b> - Licensed for Use Only with Unreal Engine-based Products",
        "isFeatured": false,
        "isCatalogItem": false,
        "categories": [
          {
            "path": "learn/games",
            "name": "UE Game Samples"
          }
        ],
        "bundle": false,
        "releaseInfo": [
          {
            "id": "036faabcbadf404eb926fc3b7dff2633",
            "appId": "Cropout_5.2",
            "compatibleApps": ["UE_5.2"],
            "platform": ["Windows", "Mac", "Linux"],
            "dateAdded": "2023-06-26T17:22:00.000Z"
          }
        ],
        "platforms": [
          {
            "key": "windows",
            "value": "Windows 64-bit"
          }
        ],
        "compatibleApps": ["5.2"],
        "urlSlug": "cropout-sample-project",
        "purchaseLimit": 1,
        "customAttributes": {},
        "tax": 0,
        "tags": [],
        "commentRatingId": "aab9066e3e644652873d24900f8dd84f",
        "ratingId": "dca36a5516154449bcc07b25834a1e00",
        "klass": "",
        "isNew": false,
        "free": true,
        "discounted": false,
        "featured": "https://cdn1.epicgames.com/item/ue/Featured_894x488-c65b7da2d8757ec48bf68806a3322e62",
        "thumbnail": "https://cdn1.epicgames.com/item/ue/image2_284x284-465de127e431017e1bf602ff0aadebb3",
        "learnThumbnail": "https://cdn1.epicgames.com/item/ue/Featured_894x488-c65b7da2d8757ec48bf68806a3322e62",
        "headerImage": "https://cdn1.epicgames.com/item/ue/Cropout_001_1920x1080-86f5b21a03b085abcae419ac4633fd79",
        "status": "ACTIVE",
        "price": "$0.00",
        "discount": null,
        "discountPrice": null,
        "ownedCount": 0,
        "canPurchase": true,
        "owned": false,
        "reviewed": false
      }
    ],
    "paging": {
      "count": 10,
      "start": 0,
      "total": 175
    },
    "sellerProfile": {
      "id": "o-aa83a0a9bc45e98c80c1b1c9d92e9e",
      "noAi": false,
      "owner": "311cffd7000046919e47765426990332",
      "status": "ACTIVE",
      "accepted": [
        {
          "ns": "ue",
          "custom": false
        }
      ],
      "financeCheckExempted": true,
      "name": "Epic Games",
      "supportEmail": "marketplace-support@unrealengine.com"
    }
  }
}
```
