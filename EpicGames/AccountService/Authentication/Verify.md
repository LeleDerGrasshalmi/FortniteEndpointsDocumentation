## Account Service - Auth: Verify

URL: https://account-public-service-prod.ol.epicgames.com/account/api/oauth/verify \
Method: GET \
Auth Required: Yes

### Query Parameters

`includePerms`: boolean (optional), if the `perms` field should be included (Defaults to `false`)

---

_Example Response (shortened)_

```json
{
  "token": "***",
  "session_id": "****",
  "token_type": "bearer",
  "client_id": "34a02cf8f4414e29b15921876da36f9a",
  "internal_client": true,
  "client_service": "launcher",
  "account_id": "94b1569506b04f9f8557af611e8c5e47",
  "expires_in": 16462,
  "expires_at": "2023-06-11T02:35:48.010Z",
  "auth_method": "exchange_code",
  "display_name": "lele stw moment",
  "app": "launcher",
  "in_app_id": "94b1569506b04f9f8557af611e8c5e47",
  "perms": [
    {
      "resource": "launcher:download:live",
      "action": 2
    },
    {
      "resource": "catalog:shared:*",
      "action": 2
    }
  ]
}
```
