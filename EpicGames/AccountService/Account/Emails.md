## Account Service - Get Emails

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId/email <br/>
Method: GET <br/>
Auth Required: Yes (`account:public:account:email READ`)

## Path Parameters

`accountId`: The target account id

---

*Example Response*

```json
{
    "accountId": "3de909f841c14552aef616973dc680a1",
    "emails": [
        {
            "email": "s.censor123@gmail.com",
            "verified": true,
            "default": true
        }
    ],
    "lastEmailUpdate": "2024-06-15T08:21:01.412Z",
    "canUpdateEmail": true
}
```
