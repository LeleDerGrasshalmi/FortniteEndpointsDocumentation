## UE Marketplace - Review Rating

URL: https://www.unrealengine.com/marketplace/api/review/:offerId/rating \
Method: GET \
Auth Required: No

## Path Parameters

`offerId`: The Id of the Offer

---

_Example Response_

```json
{
  "status": "OK",
  "data": {
    "targetId": "a3d91055eb4b475ebe9ce9c60dd682a9",
    "averageRating": 5,
    "rating5": 1,
    "rating4": 0,
    "rating3": 0,
    "rating2": 0,
    "rating1": 0,
    "answeredQuestion": 1,
    "totalQuestion": 2,
    "legacyRatingNum": 0,
    "total": 1,
    "rating5Percent": 100,
    "rating4Percent": 0,
    "rating3Percent": 0,
    "rating2Percent": 0,
    "rating1Percent": 0
  }
}
```
