## Fortnite Website - Account Info

URL: https://www.fortnite.com/:locale/api/accountInfo \
Method: GET \
Auth Required: Yes

## Path Parameters

`locale`: Doesn't matter in this context, just use `en-US`

---

_Example Response (logged in)_

```json
{
  "isLoggedIn": true,
  "accountInfo": {
    "id": "94b1569506b04f9f8557af611e8c5e47",
    "displayName": "lele stw moment",
    "email": "lele@example.com",
    "country": "DE",
    "isLoggedIn": true,
    "lastName": "",
    "name": "",
    "lang": "de",
    "cabinedMode": false
  }
}
```

_Example Response (not logged in)_

```json
{
  "accountInfo": {}
}
```
