## Account Web - Orders

URL: https://www.epicgames.com/account/v2/subscription/orders \
Method: GET \
Auth Required: Yes

_Example Response_

```json
{
  "elements": [
    {
      "id": "#####",
      "identityId": "#####",
      "orderType": "PURCHASE",
      "orderStatus": "COMPLETED",
      "subscriptionId": "#####",
      "totalDiscounted": 1199,
      "basePrice": 1199,
      "vatAmount": 208,
      "totalTax": 0,
      "currency": "EUR",
      "invoiceId": "#####",
      "convenienceFee": 0,
      "completedAt": "2023-03-31T20:28:20.596+0000",
      "createdAt": "2023-03-31T20:28:13.472+0000",
      "billingAccountId": "#####",
      "billingAccountName": "Visa - 0000",
      "totalPrice": 1199,
      "namespace": "fn",
      "offerId": "9ec21a8d4f744f8b938fbf79d02d40b9",
      "orderTransactionInfo": {
        "transactionId": "#####",
        "gatewayType": "CHASE",
        "paymentMethodType": "CREDITCARD",
        "paymentMethodSubtype": "VISA"
      },
      "countryCode": "ES",
      "offerTitle": "Fortnite Crew",
      "presentmentBasePrice": "€11.99",
      "priceString": "€11.99",
      "presentmentConvenienceFee": "€0.00",
      "presentmentTotalTax": "€0.00",
      "createdAtMillis": 1680294493472
    }
  ],
  "paging": {
    "start": 0,
    "count": 10,
    "total": 1
  }
}
```