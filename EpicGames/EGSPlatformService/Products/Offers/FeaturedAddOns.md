## EGS Platform Service - Product Featured Add Ons

URL: https://egs-platform-service.store.epicgames.com/api/v1/egs/products/:productId/featured-offers/add-ons \
Method: GET \
Auth Required: No

## Query Parameters

`count`: (required) element count to return <br/>
`country`: (required) ISO 3166 - Alpha 2 Code <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`start`: (required) start index <br/>
`store`: (required) valid Catalog Service Stores, e.g. `EGS`

## Path Parameters

`productId`: self explaining, e.g. `prod-fn` for fortnite

---

_Example Response_

```json
{
  "__typename": "PaginatedOffers",
  "data": [
    {
      "__typename": "Offer",
      "attention": {
        "earlyAccess": {
          "earlyAccess": false
        },
        "inAppPurchases": {
          "support": "None"
        },
        "nftBlockchain": {
          "nftBlockchain": false
        }
      },
      "categories": ["addons", "addons/durable"],
      "developers": ["Epic Games"],
      "id": "ce270cdcc5404dc68305158c31850013",
      "initialPcReleaseDate": 1713398400000,
      "mapping": {
        "__typename": "InternalMapping",
        "slug": "fortnite--shrieking-star-quest-pack"
      },
      "media": {
        "card16x9": {
          "imageSrc": "https://cdn1.epicgames.com/offer/fn/EN_29_2560x1440-a719ea7c71767a677dcf06e418f25829"
        },
        "card3x4": {
          "imageSrc": "https://cdn1.epicgames.com/offer/fn/EN_29_1200x1600-d48ee6445243f0086278062e5f136d86"
        }
      },
      "productId": "prod-fn",
      "publishers": ["Epic Games"],
      "purchase": [
        {
          "offerLifecycleState": "Release",
          "priceDisplay": "$8.99",
          "purchasePayload": {
            "offerId": "ce270cdcc5404dc68305158c31850013",
            "sandboxId": "fn"
          },
          "purchaseStateEffectiveDate": 1715510520000,
          "status": "AvailableToPurchase"
        },
        {
          "offerEffectivenessState": "Expired",
          "purchasePayload": {
            "offerId": "ce270cdcc5404dc68305158c31850013",
            "sandboxId": "fn"
          },
          "purchaseStateEffectiveDate": 1715731200000,
          "status": "Unavailable"
        }
      ],
      "refundType": "NonRefundable",
      "releaseDate": {
        "timestamp": 1713398400000,
        "type": "ExactDate"
      },
      "shortDescription": "Rise from the ancient myths to reach for the shrieking stars. Includes an Outfit (with LEGO® Style), Back Bling, Pickaxe and Quests to earn up to 1,000 V-Bucks.",
      "store": "EGS",
      "subscription": {
        "__typename": "SubscriptionUnsupported"
      },
      "tags": {
        "accessibility": [],
        "epicFeatures": [],
        "events": [],
        "features": [],
        "genres": [],
        "platforms": [],
        "usersSay": []
      },
      "title": "Shrieking Star Quest Pack"
    }
  ],
  "paging": {
    "count": 1,
    "start": 0,
    "total": 11
  }
}
```
