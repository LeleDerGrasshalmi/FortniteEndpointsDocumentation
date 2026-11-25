# RecycleItem

**Description**: `Recycle a Item` <br/>
**Profiles**: `campaign`

## Body

```js
{
    "targetItemId": "" // Item GUID
}
```

## Notifications

| Notification Type                                    | Description                                                            |
| ---------------------------------------------------- | ---------------------------------------------------------------------- |
| [slotItemResult](../Notifications/slotItemResult.md) | If the item was Collected, this will have the UUID of the slotted item |
