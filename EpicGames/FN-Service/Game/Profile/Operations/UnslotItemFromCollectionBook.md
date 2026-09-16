# UnslotItemFromCollectionBook

**Description**: `Remove an item from the Collection Book and get the item back into ur inventory` ([This](https://cdn.discordapp.com/attachments/842511284469366824/922575625632501830/unknown.png)) \
**Profiles**: `campaign`

## Body

```js
{
    "templateId": "", // Item TemplateId
    "itemId": "", // Item GUID
    "specific": "" // Leave as an empty string
}
```

## Notifications

| Notification Type                                                        | Description                         |
| ------------------------------------------------------------------------ | ----------------------------------- |
| [collectionBookUnslotItem](../Notifications/collectionBookUnslotItem.md) | Contains UUID of the Unslotted Item |