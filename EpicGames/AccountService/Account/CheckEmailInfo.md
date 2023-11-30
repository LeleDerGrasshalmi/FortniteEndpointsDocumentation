## Account Service - Check Account Email Info

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId/email \
Method: GET \
Auth Required: Yes (`account:public:account:email READ`)

## Path Parameters

`accountId`: The target account id

---

_Example Response_

```json
{
    "accountId": "d3663f8de4664a9191034bf921d537fc",
    "emails": [
        {
            "email": "ylsdev@example.com",
            "verified": false,
            "default": true
        }
    ],
    "canUpdateEmail": true
}
```
