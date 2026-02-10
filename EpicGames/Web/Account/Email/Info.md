## Account Web - Email: Info

URL: https://www.epicgames.com/account/v2/api/email/info \
Method: GET \
Auth Required: Yes

---

_Example Response_

```json
{
  "isSuccess": true,
  "data": {
    "canUpdateEmail": true,
    "canUpdateNext": "",
    "default": {
      "email": "lele@example.com",
      "verified": true,
      "default": true
    },
    "lastEmailUpdate": null,
    "unverified": null
  }
}
```
