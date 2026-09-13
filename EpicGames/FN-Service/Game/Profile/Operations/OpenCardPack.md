# OpenCardPack

**Description**: `Open a CardPack (Llama, Chest, ...)` \
**Profiles**: `campaign`

## Body

```js
{
    "cardPackItemId": "", // Cardpack Item GUID
    "selectionIdx": 0 // If theres multiple Rewards, the Index of the selected Reward
}
```

## Notifications

| Notification Type                                    | Description                                                                     |
| ---------------------------------------------------- | ------------------------------------------------------------------------------- |
| [cardPackResult](../Notifications/cardPackResult.md) | Lists contents of the opened CardPack                                           |
| [phoenixLevelUp](../Notifications/phoenixLevelUp.md) | One of these will be present for every Level Up caused by obtaining Ventures XP |