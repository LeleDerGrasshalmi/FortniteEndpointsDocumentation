## EGS Platform Service - Product Offer Age Rating

URL: https://egs-platform-service.store.epicgames.com/api/v1/egs/products/:productId/featured-offers/add-ons \
Method: GET \
Auth Required: No

## Query Parameters

`count`: (required) element count to return <br/>
`country`: (required) ISO 3166 - Alpha 2 Code <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`start`: (required) start index <br/>
`store`: (required) only `EGS` is known to be valid

## Path Parameters

`productId`: self explaining, e.g. `prod-fn` for fortnite

---

_Example Response (heavily shortened)_

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
            "categories": [
                "addons",
                "addons/durable"
            ],
            "developers": [
                "Epic Games"
            ],
            "id": "be3b61686d044d86bf7fb5fa46284681",
            "initialPcReleaseDate": 1703289600000,
            "mapping": {
                "__typename": "InternalMapping",
                "slug": "fortnite--gilded-elites-pack"
            },
            "media": {
                "card16x9": {
                    "imageSrc": "https://cdn1.epicgames.com/offer/fn/EN_S28_GildedElitesPack_EGS_Launcher_2560x1440_2560x1440-4d642ed71c80556d2fa87264453647a7"
                },
                "card3x4": {
                    "imageSrc": "https://cdn1.epicgames.com/offer/fn/EN_S28_GildedElitesPack_EGS_Launcher_1200x1600_1200x1600-05ce561964d2f7985dc195dfbe3e0eb0"
                }
            },
            "productId": "prod-fn",
            "publishers": [
                "Epic Games"
            ],
            "purchase": [
                {
                    "offerLifecycleState": "Release",
                    "priceDisplay": "$17.25",
                    "purchasePayload": {
                        "offerId": "be3b61686d044d86bf7fb5fa46284681",
                        "sandboxId": "fn"
                    },
                    "purchaseStateEffectiveDate": 1703633580000,
                    "status": "AvailableToPurchase"
                },
                {
                    "offerEffectivenessState": "Expired",
                    "purchasePayload": {
                        "offerId": "be3b61686d044d86bf7fb5fa46284681",
                        "sandboxId": "fn"
                    },
                    "purchaseStateEffectiveDate": 1707523200000,
                    "status": "Unavailable"
                }
            ],
            "refundType": "NonRefundable",
            "releaseDate": {
                "timestamp": 1703289600000,
                "type": "ExactDate"
            },
            "shortDescription": "They've got one thing in common and it happens to be the one thing they all adore. Includes 3 Outfits (with LEGO® Styles), 3 Back Blings and 3 Pickaxes.",
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
            "title": "Gilded Elites Pack"
        }
    ],
    "paging": {
        "count": 999,
        "start": 1,
        "total": 9
    }
}
```
