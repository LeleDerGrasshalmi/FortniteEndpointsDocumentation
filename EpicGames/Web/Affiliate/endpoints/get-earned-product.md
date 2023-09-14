# Get Earned Products

URL: https://sac.epicgames.com/api/get-earned-products \
Method: GET \
Auth Required: Yes

## Query Parameters

`date`: Format: `YYYY-MM`, e.g. `2023-09`, <br/>
`locale`: Content Language, e.g. `de`, `en-US`

---

_Example Response_

```json
{
  "data": {
    "fortnite": {
      "namespace": "fortnite",
      "data": [
        {
          "date": "2023-09-14",
          "referrals": 333,
          "avgShareRate": 0,
          "currency": "USD"
        }
      ],
      "totalUniqueSupporters": 333,
      "totalEstimatedEarnings": 0,
      "title": "Fortnite",
      "icon": "https://cdn1.epicgames.com/offer/fn/26BR_C4S4_EGS_Launcher_Blade_1200x1600_1200x1600-72d477839e2f1e1a9b3847d0998f50bc",
      "link": null,
      "shareRate": 5,
      "urlSlug": "fortnite",
      "pageSlug": "fortnite"
    }
  },
  "success": true
}
```
