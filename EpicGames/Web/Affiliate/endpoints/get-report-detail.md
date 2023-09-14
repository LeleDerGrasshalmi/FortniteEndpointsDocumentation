# Get Report Details

URL: https://sac.epicgames.com/api/v1/get-report-detail \
Method: GET \
Auth Required: Yes

## Query Parameters

`paymentId`: Payment Id (from the [List](./get-report-list.md))

---

_Example Response_

```json
{
  "data": {
    "elements": [
      {
        "reportId": "3dda5915493c4e15abbe2a94fe1f78cf",
        "notes": "Revenue earned for 2023-09-01",
        "amount": 10099,
        "period": "2023-09"
      }
    ],
    "paging": {
      "count": 30,
      "start": 0
    },
    "paymentId": "3f8c0cf81f7f45f09d081f44e0168941"
  },
  "success": true
}
```
