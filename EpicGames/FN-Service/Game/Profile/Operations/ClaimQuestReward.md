# ClaimQuestReward

**Description**: `Claim a Quest Reward` \
**Profiles**: `athena`, `campaign`

## Body

```js
{
    "questId": "", // Quest Item GUID
    "selectedRewardIndex": 0 // If there is a choice between reward the selected rewards index
}
```

## Notifications

| Notification Type                            | Description                    |
| -------------------------------------------- | ------------------------------ |
| [questClaim](../Notifications/questClaim.md) | Lists rewards of claimed Quest |