# OpenCardPackBatch

**Description**: `Open CardPacks [e.g. Llamas, Chests] (Bulk)` \
**Profiles**: `campaign`

## Body

```js
{
    "cardPackItemIds": [] // Cardpack Item GUIDs
}
```

## Notifications

| Notification Type                                    | Description                                                                     |
| ---------------------------------------------------- | ------------------------------------------------------------------------------- |
| [cardPackResult](../Notifications/cardPackResult.md) | Lists contents of all opened CardPacks                                          |
| [phoenixLevelUp](../Notifications/phoenixLevelUp.md) | One of these will be present for every Level Up caused by obtaining Ventures XP |