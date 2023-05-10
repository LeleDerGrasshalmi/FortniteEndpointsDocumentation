## EGS Platform Service - Category Cards

URL: https://egs-platform-service.store.epicgames.com/api/v1/egs/category-cards \
Method: GET \
Auth Required: No

## Query Parameters

`count`: (required) 1 <= 999 <br/>
`country`: (required) ISO 3166 - Alpha 2 Code <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`start`: (required) start index <br/>
`store`: (required) only `EGS` is known to be valid <br/>

---

Example Response

```json
{
  "data": [
    {
      "images": [
        "https://cdn1.epicgames.com/offer/48e20c81667c4ff49c85dd79ac3a01b0/EGS_Redfall_ArkaneStudios_S2_1200x1600-2f567c0dbf7e69015b741fc9b52c8b91_1200x1600-2f567c0dbf7e69015b741fc9b52c8b91",
        "https://cdn1.epicgames.com/spt-assets/140874c6dacd4012b94d3858a64091bc/rice-cj0l8.png",
        "https://cdn1.epicgames.com/spt-assets/2e5c85a5931548f69839b539d214ef81/city-of-beats-13s3n.jpg"
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
