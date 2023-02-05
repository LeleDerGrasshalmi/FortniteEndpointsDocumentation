# StorageTransfer

**Description**: `Transfer items from/to the Storage` \
**Profiles**: `theater0`

## Body
```js
{
    "transferOperations": [{
        "itemId": "", // Item GUID
        "quantity": 1, // Item Quantity
        "toStorage": false, // Whether its into the inventory/backpack (then false) if into the storage then true
        "newItemIdHint": "" // Leave empty
    }]
}
```
