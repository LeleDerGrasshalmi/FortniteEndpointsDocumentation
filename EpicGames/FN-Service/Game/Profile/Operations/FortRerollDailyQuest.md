# FortRerollDailyQuest

**Description**: `Reroll a Daily Quest` <br/>
**Profiles**: `athena`, `campaign`

## Body

```js
{
    "questId": "" // Quest Item GUID
}
```

## Notifications

| Notification Type                                        | Description                                                     |
| -------------------------------------------------------- | --------------------------------------------------------------- |
| [dailyQuestReroll](../Notifications/dailyQuestReroll.md) | Contains the Quest Template ID that the Quest was rerolled into |
