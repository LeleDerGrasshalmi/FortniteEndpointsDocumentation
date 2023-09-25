## Account Web - Subscription: Order

URL: https://www.epicgames.com/account/v2/subscription/order-detail \
Method: GET \
Auth Required: Yes

## Query Parameters

`orderId`: The Id of the Subscription Order

---

_Example Response_

```json
{
  "id": "94b1569506b04f9f8557af611e8c5e47",
  "identityId": "94b1569506b04f9f8557af611e8c5e47",
  "country": "ES",
  "orderType": "PURCHASE",
  "orderStatus": "COMPLETED",
  "orderReason": "INITIAL_BUY",
  "subscriptionDefId": "#####",
  "orgId": "o-aa83a0a9bc45e98c80c1b1c9d92e9e",
  "subscriptionDefLevelId": "#####",
  "billingCycle": "MONTHLY",
  "subscriptionId": "#####",
  "namespace": "fn",
  "offerId": "9ec21a8d4f744f8b938fbf79d02d40b9",
  "totalDiscounted": 1199,
  "basePrice": 1199,
  "basePayoutPrice": 1081,
  "basePayoutCurrencyCode": "USD",
  "revenueWithoutTax": 1081,
  "vatAmount": 208,
  "vatRate": 0.21,
  "totalTax": 0,
  "taxType": "Tax",
  "currency": "EUR",
  "receiptId": "#####",
  "invoiceId": "#####",
  "taxStatus": "SUCCEEDED",
  "convenienceFee": 0,
  "fraud": false,
  "fraudDecision": "CHALLENGE_3DS",
  "fraudSubDecisions": ["3DS_LOW_VALUE_EXEMPTION"],
  "merchantGroup": "FN_MKT",
  "morId": "#####",
  "salesChannelId": "fngame-purchase-client",
  "completedAt": "2023-03-31T20:28:20.596+0000",
  "createdAt": "2023-03-31T20:28:13.472+0000",
  "refundedAmount": 0,
  "chargebackAmount": 0,
  "billingAccountId": "#####",
  "billingAccountName": "Visa - 0000",
  "totalPrice": 1199,
  "toSettle": true,
  "sendReceipt": true,
  "accountIpAddress": "#####",
  "accountIpCountry": "ES",
  "entitlementSource": "eos",
  "offerTitle": "Fortnite Crew",
  "eventDiscount": 0,
  "submittedTax": 208,
  "toUsdExchangeRate": 1.0904880371404575,
  "zipcode": "",
  "state": "",
  "city": "",
  "offerInfo": {
    "offerId": "9ec21a8d4f744f8b938fbf79d02d40b9",
    "title": "Fortnite Crew",
    "quantity": 1,
    "totalPrice": 1199,
    "unitPrice": 1199,
    "basePrice": 1199,
    "taxPrice": 0,
    "discountedPrice": 1199,
    "basePayoutCurrencyCode": "USD",
    "basePayoutPrice": 1199,
    "revenueWithoutTax": 1199,
    "namespace": "fn",
    "namespaceDisplayName": "Fortnite",
    "sellerId": "o-aa83a0a9bc45e98c80c1b1c9d92e9e",
    "sellerName": "Epic Games",
    "vat": 0,
    "convenienceFee": 0,
    "voucherDiscount": 0
  },
  "resendReceipt": true,
  "isB2bVatReverseCharge": true,
  "vatEnabled": true,
  "paymentCurrencyAmount": 1199,
  "paymentCurrencyCode": "EUR"
}
```
