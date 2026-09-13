# RecycleItemBatch

**Description**: `Recycle Items (Bulk)` \
**Profiles**: `campaign`

## Body

```js
{
    "targetItemIds": [] // Item GUIDs
}
```

## Notifications

| Notification Type                                    | Description                                                                               |
| ---------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| [slotItemResult](../Notifications/slotItemResult.md) | One of these will be returned for every Collected item, containing the slotted items UUID |