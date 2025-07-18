## Redeem Web - Ratings

URL: https://redeem.epicgames.com/api/product/age-rating \
Method: GET \
Auth Required: No

## Query Parameters

`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`country`: (required) ISO 3166 - Alpha 2 Code

---

_Example Response_

```json
{
  "data": {
    "__typename": "AgeRating",
    "ageControl": 0,
    "contentDescriptors": [
      "Violence",
      "Online Interactivity"
    ],
    "interactiveElements": [
      "Users Interact",
      "In-Game Purchases"
    ],
    "ratingImage": "https://cdn1.epicgames.com/gameRating/gameRating/ACB_M_192_192x192-b702f1ebcbc6daa7458356527d4bba16",
    "ratingSystem": "ACB",
    "title": "Mature"
  }
}
```
