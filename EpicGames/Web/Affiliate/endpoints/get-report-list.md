# Get Report List

URL: https://sac.epicgames.com/api/v1/get-report-list \
Method: GET \
Auth Required: Yes

## Query Parameters

`start`: Offset (paging) <br/>
`count`: Count of elements to return

---

_Example Response_

```json
{
  "data": {
    "elements": [
      {
        "paymentId": "3f8c0cf81f7f45f09d081f44e0168941",
        "amount": 10099,
        "paymentCreateDate": "2023-09-14T17:03:19.034+0000",
        "payeeId": "0d2ccb730f2f4fac82d04bb7bb8d2d80",
        "earnerId": "0d2ccb730f2f4fac82d04bb7bb8d2d80",
        "notes": "AFFILIATE Payout - INT - Sep 2023",
        "status": "COMPLETED"
      }
    ],
    "paging": {
      "count": 10,
      "start": 0,
      "total": 6
    }
  },
  "success": true
}
```
