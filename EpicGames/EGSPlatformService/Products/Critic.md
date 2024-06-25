## EGS Platform Service - Product Critic

URL: https://egs-platform-service.store.epicgames.com/api/v1/egs/products/:productId/critic-reviews/open-critic \
Method: GET \
Auth Required: No

## Query Parameters

`count`: (required) self explaining <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`start`: (required) start index <br/>
`store`: (required) valid Catalog Service Stores, e.g. `EGS`

## Path Parameters

`productId`: self explaining, e.g. `prod-fn` for Fortnite

---

_Example Response_

```json
{
  "__typename": "ProductCriticReviewsEnabled",
  "criticReviews": {
    "__typename": "CriticReviews",
    "criticAverage": 84,
    "criticRating": "Mighty",
    "recommendPercentage": 93,
    "reviews": {
      "__typename": "PaginatedCriticReviews",
      "data": [
        {
          "author": "Ford James",
          "body": "Nobody thought Fortnite would still be popular this late on, but it's continued to adapt and fight for its spot at the top of the battle royale ladder.",
          "outlet": "GamesRadar+",
          "score": {
            "__typename": "CriticReviewStarScore",
            "earnedStars": 4,
            "totalStars": 5
          },
          "url": "https://www.gamesradar.com/fortnite-review/"
        }
      ],
      "paging": {
        "count": 1,
        "start": 0,
        "total": 3
      }
    },
    "url": "https://opencritic.com/game/6228/fortnite-battle-royale"
  }
}
```
