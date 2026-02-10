## Account Web - Order History

URL: https://www.epicgames.com/account/v2/payment/ajaxGetOrderHistory \
Method: GET \
Auth Required: Yes

---

_Example Response_

```json
{
   "orders":[
      {
         "orderType":"PURCHASE",
         "canSendReceipt":false,
         "orderId":"F2405272344201295",
         "createdAtMillis":1716852860288,
         "items":[
            {
               "description":"Discord Nitro",
               "quantity":1,
               "amount":"CA$0.00",
               "price":0,
               "offerId":"55ba24c34b87463a966d186f26835665",
               "namespace":"5f3c898b2a3244af99e9900e015717f8"
            }
         ],
         "merchantGroup":"EGS_MKT",
         "transactions":[
            
         ],
         "subtotal":0,
         "tax":0,
         "convenienceFee":0,
         "total":0,
         "presentmentSubtotal":"CA$0.00",
         "presentmentTax":"CA$0.00",
         "presentmentConvenienceFee":"CA$0.00",
         "presentmentTotal":"CA$0.00",
         "promotions":[
            
         ],
         "marketplaceName":"Epic Games Store"
      }
]
}
```
