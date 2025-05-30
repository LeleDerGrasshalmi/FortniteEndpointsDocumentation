## Account Service - Get Email

URL: https://account-public-service-prod.ol.epicgames.com/account/api/accounts/:accountId/email \
Method: GET \
Auth Required: Yes

## Path Parameters

`accountId`: The target account id

---

_Example Response_

```json
{
    "accountId": "3de909f841c14552aef616973dc680a1",
    "email": {
            "email": "s.censor123@gmail.com",
            "verified": true,
            "default": true
    },
    "lastEmailUpdate": "2024-06-15T08:21:01.412Z",
    "canUpdateEmail": true
}
```
