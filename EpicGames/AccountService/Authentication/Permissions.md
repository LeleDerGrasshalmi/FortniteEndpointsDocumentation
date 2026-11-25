## Account Service - Auth: Permissions

URL: https://account-public-service-prod.ol.epicgames.com/account/api/oauth/permissions <br/>
Method: GET <br/>
Auth Required: Yes

---

*Example Response (shortened)*

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
