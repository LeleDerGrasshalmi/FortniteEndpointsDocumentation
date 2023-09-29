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

---

_Example Response_

- Status 200: Player exist and got a leaderboard entry for the eventId and eventWindowId
- Status 404: Player exist, but got no leaderboard entry for the eventId and eventWindowId
- Status 500: Player doesn't exist or got unsupported characters in their name (currently spaces are known as such)
