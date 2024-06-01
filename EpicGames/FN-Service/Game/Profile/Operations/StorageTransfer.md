# StorageTransfer

**Description**: `Transfer items from/to the Storage` \
**Profiles**: `theater0`

## Body

```js
{
    "transferOperations": [{
        "itemId": "", // Item GUID
        "quantity": 1, // Item Quantity
        "toStorage": false, // Whether its into the Inventory/Backpack (then false), or into the Storage (then true)
        "newItemIdHint": "" // Item GUID to stack the Items to
    }]
}
```
