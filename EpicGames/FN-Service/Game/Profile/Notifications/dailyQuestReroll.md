# dailyQuestReroll

**Description**: `The new Quest that replaces the Rerolled Quest` \
**Operations**: [FortRerollDailyQuest](../Operations/FortRerollDailyQuest.md)

## Body

```js
{
   // standard profile notification content
   "type": "dailyQuestReroll",
   "primary": true,
   "client_request_id": "",

   //specific to this notification
   "questId": "Quest:quest_s42_cosmicthunder_00_promo_q22"
}
```