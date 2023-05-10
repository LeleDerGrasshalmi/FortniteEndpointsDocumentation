## EGS Platform Service - Product Offer Age Rating

URL: https://egs-platform-service.store.epicgames.com/api/v1/egs/products/:productId/offers/:offerId/age-rating \
Method: GET \
Auth Required: No

## Query Parameters

`country`: (required) ISO 3166 - Alpha 2 Code <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`store`: (required) only `EGS` is known to be valid <br/>

## Path Parameter

`productId`: self explaining, e.g. `7c0a8a40ba4a47dd899eed51a8fbc3fe` for Rogue Company <br/>
`offerId`: self explaining, e.g. `36bfbc7a0b664a2891c68dc947922469` for the Rogue Company Main Offer <br/>

---

Example Response

```json
{
  "__typename": "AgeRating",
  "ageGate": {
    "gate": "no-gate"
  },
  "ageRating": {
    "ageControl": 16,
    "contentDescriptors": [],
    "interactiveElements": [],
    "ratingImage": "https://cdn1.epicgames.com/salesEvent/salesEvent/esr_16_390x450-904d1ed3d452c95f3d86a8f56e6cd62f",
    "ratingSystem": "EPIC SUGGESTED RATING",
    "title": "16+"
  }
}
```
