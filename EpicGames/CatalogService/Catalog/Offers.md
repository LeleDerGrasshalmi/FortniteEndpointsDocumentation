## Catalog Service - Catalog: Offers

URL: https://catalog-public-service-prod06.ol.epicgames.com/catalog/api/shared/namespace/:namespace/offers \
Method: GET \
Auth Required: Yes

## Path Parameters

`namespace`: The Catalog Namespace, e.g. `fn` for Fortnite

## Query Parameters

`country`: e.g. `US` <br/>
`locale`: e.g. `en` <br/>
`returnItemDetails`: (bool), e.g. `false` <br/>
`count`: Maximum returned offers, e.g. `10`

---

_Example Response (shortened)_

```json
{
  "metadata": {},
  "elements": [
    {
      "id": "8b620ab6eaad4c6182d44f07830fd8f6",
      "title": "Aztez",
      "description": "Aztez is a unique hybrid of beat 'em up and turn-based strategy, set in the world of the Aztec Empire. ...",
      "keyImages": [],
      "categories": [
        {
          "path": "games"
        },
        {
          "path": "games/edition/base"
        },
        {
          "path": "games/edition"
        },
        {
          "path": "applications"
        }
      ],
      "namespace": "5b325322a4c04b9e9e780b9a1e9b2d70",
      "status": "ACTIVE",
      "internalName": "Aztez",
      "items": [
        {
          "id": "fc5c077c77604e96ab1704acec3d542a",
          "keyImages": [],
          "categories": [],
          "namespace": "5b325322a4c04b9e9e780b9a1e9b2d70",
          "unsearchable": false
        }
      ],
      "currencyCode": "USD",
      "currentPrice": 1999,
      "seller": {
        "id": "o-ndzqj36dmhqmfklcq44yywpgfnbmbd",
        "name": "Team Colorblind"
      },
      "tags": [1216, 1344, 1370, 9549, 1263],
      "offerType": "BASE_GAME",
      "releaseDate": "2020-02-06T16:00:00.000Z",
      "urlSlug": "gruntgeneralaudience",
      "publisherDisplayName": "Team Colorblind",
      "developerDisplayName": "Team Colorblind",
      "supportedPlatforms": ["Windows", "macOS"]
    }
  ],
  "paging": {
    "count": 10,
    "start": 0,
    "total": 2
  }
}
```
