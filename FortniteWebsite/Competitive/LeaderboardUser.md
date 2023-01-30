## Fortnite Website - Competitive Leaderboard User

URL: https://www.fortnite.com/competitive/api/leaderboard/:eventId/:eventWindowId/undefined \
Method: POST \
Auth Required: No

Payload:

```js
{
    "name": "krowemoh"
}
```
Status codes:
- 200: Player exist and got a leaderboard entry for the eventId and eventWindowId
- 404: Player exist, but got no leaderboard entry for the eventId and eventWindowId
- 500: Player doesn't exist or got unsupported characters in their name (currently spaces are known as such)
