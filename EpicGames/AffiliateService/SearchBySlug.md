## Affiliate Service - Affiliates: Search by Slug

Search Support-A-Creator codes (slugs) that start with a term. Results are sorted alphabetically by slug, an exact match comes first.

URL: https://affiliate-public-service-prod.ol.epicgames.com/affiliate/api/public/affiliates/search \
Method: GET \
Auth Required: Yes (`affiliate:public:affiliate READ`)

## Query Parameters

`slugSearchTerm`: (required), the prefix to search for, at least 3 characters <br/>
`start`: (optional), offset for paging, defaults to `0` <br/>
`count`: (optional), page size, defaults to `30`

---

_Example Response (shortened, `slugSearchTerm=ninja&count=3`)_

```json
{
  "elements": [
    {
      "id": "4735ce9132924caf8a5b17789b40f79c",
      "slug": "ninja",
      "displayName": "Ninja",
      "status": "ACTIVE",
      "verified": false
    },
    {
      "id": "63dab037d43b494c9449cb605e916cdc",
      "slug": "ninja007tv",
      "displayName": "TTV NINJA_007TV",
      "status": "ACTIVE",
      "verified": false
    }
  ],
  "paging": {
    "count": 3,
    "start": 0,
    "total": 72
  }
}
```

_Example Response (term shorter than 3 characters or missing, `400`)_

```json
{
  "errorCode": "errors.com.epicgames.ecommerce.affiliate.invalid_slug_search_term",
  "errorMessage": "slugSearchTerm [ni] has to be at least three letters",
  "messageVars": ["ni"],
  "numericErrorCode": 47033,
  "originatingService": "com.epicgames.ecp",
  "intent": "prod"
}
```
