# StorageTransfer

**Description**: `Transfer items from/to the Storage` \
**Profiles**: `theater0`

## Body
```js
{
    "transferOperations": [{
        "itemId": "", //item guid
        "quantity": 1, //item quantity
        "toStorage": false, //whether its into the inventory/backpack (then false) if into the storage then true
        "newItemIdHint": "" //leave empty
    }]
}
```
