## Launcher Service - Payment: Default Billing-Account

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/payment/accounts/:accountId/billingaccounts/default <br/>
Method: GET <br/>
Auth Required: Yes (`payment:public:{accountId}:billingaccount:default READ`)

## Path Parameters

`accountId`: Your Account Id

---

*Example Response*

```json
{
  "country": "DE",
  "countrySource": "ACCOUNT",
  "currency": "EUR"
}
```
