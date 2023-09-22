## Account Web - Security TFA: Info

URL: https://www.epicgames.com/account/v2/security/settings/ajaxGet \
Method: GET \
Auth Required: Yes

---

_Example Response_

```json
{
  "isSuccess": true,
  "settings": {
    "enabled": true,
    "defaultMethod": "authenticator",
    "methods": {
      "authenticator": {
        "name": "authenticator",
        "enabled": true,
        "verified": true
      },
      "email": {
        "name": "email",
        "enabled": true,
        "verified": true
      }
    }
  }
}
```
