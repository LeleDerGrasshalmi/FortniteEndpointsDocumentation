## EGS Platform Service - Category Cards

URL: https://egs-platform-service.store.epicgames.com/api/v1/egs/category-cards \
Method: GET \
Auth Required: No

## Query Parameters

`count`: (required) 1 <= 999 <br/>
`country`: (required) ISO 3166 - Alpha 2 Code <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`start`: (required) start index <br/>
`store`: (required) valid Catalog Service Stores, e.g. `EGS`

---

_Example Response_

```json
{
  "__typename": "PaginatedCategoryCards",
  "data": [
    {
      "images": [
        "https://cdn1.epicgames.com/spt-assets/01bd1b95902f4a73b04267c0e17161a5/spellbound-survivors-v4auq.jpg",
        "https://cdn1.epicgames.com/spt-assets/c97bd69018fc427d98808d1435bcc503/garten-of-banban-7-170tp.png",
        "https://cdn1.epicgames.com/spt-assets/ed48f0c4ab5640b0bc3efc8c4fe0b40b/ivorfall-1g4ao.png"
      ],
      "slug": "action-games",
      "title": "Action Games"
    }
  ],
  "paging": {
    "count": 1,
    "start": 0,
    "total": 40
  }
}
```
