# catalogPurchase

**Description**: `The item grants from a purchased Catalog Offer` \
**Operations**: [PurchaseCatalogEntry](../Operations/PurchaseCatalogEntry.md)

## Body

```js
{
   // standard profile notification content
    "type": "catalogPurchase",
    "primary": true,
    "client_request_id": "",
    
    //specific to this notification
    "lootResult": {
       "items": [
           {
              "itemType": "AccountResource:reagent_evolverarity_r",
              "itemGuid": "4b1ef7a4-cb22-427c-99aa-a6b28489428a",
              "itemProfile": "campaign",
              "quantity": 10
            }
            //...
         ]
    }
}
```
