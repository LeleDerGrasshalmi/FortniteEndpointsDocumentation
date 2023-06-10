## Account Service - Auth: Permissions

URL: https://account-public-service-prod.ol.epicgames.com/account/api/oauth/permissions \
Method: GET \
Auth Required: Yes

---

_Example Response (shortened)_

```json
[
  {
    "resource": "launcher:download:live",
    "action": 2
  },
  {
    "resource": "catalog:shared:*",
    "action": 2
  }
]
```
