## EGS Platform Service - Product Critic

URL: https://egs-platform-service.store.epicgames.com/api/v1/egs/products/:productId/critic-reviews/open-critic \
Method: GET \
Auth Required: No

## Query Parameters

`count`: (required) self explaining <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`start`: (required) start index <br/>
`store`: (required) only `EGS` is known to be valid

## Path Parameters

`productId`: self explaining, e.g. `prod-fn` for Fortnite

---

Example Response

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
        },
        {
          "author": "Austen Goslin",
          "body": "Thanks to the freedom of its outstanding building mechanic, Fortnite Battle Royale isn't just a great battle royale game – it's one of the best multiplayer games in recent history.",
          "outlet": "IGN",
          "score": {
            "__typename": "CriticReviewNumericScore",
            "earnedScore": 9.6,
            "totalScore": 10
          },
          "url": "https://www.ign.com/articles/2018/03/27/fortnite-battle-royale-review"
        },
        {
          "author": "Daniel Tack",
          "body": "Playable, watchable, understandable, and enjoyable by just about anyone with a pulse, Fortnite is an absolute blast",
          "outlet": "Game Informer",
          "score": {
            "__typename": "CriticReviewNumericScore",
            "earnedScore": 9.5,
            "totalScore": 10
          },
          "url": "https://www.gameinformer.com/review/fortnite/an-epic-epoch"
        }
      ],
      "paging": {
        "count": 3,
        "start": 0,
        "total": 3
      }
    },
    "url": "https://opencritic.com/game/6228/fortnite-battle-royale"
  }
}
```
