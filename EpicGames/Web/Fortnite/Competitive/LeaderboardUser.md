## Fortnite Website - Competitive Leaderboard User

URL: https://www.fortnite.com/competitive/api/leaderboard/:eventId/:eventWindowId/undefined <br/>
Method: POST <br/>
Auth Required: No

```json
{
    "name": "krowemoh"
}
```

## Path Parameters

`eventId`: The event ID. <br/>
`eventWindowId`: The event window ID.

---

*Example Response*

- Status 200: Player exist and got a leaderboard entry for the eventId and eventWindowId
- Status 404: Player exist, but got no leaderboard entry for the eventId and eventWindowId
- Status 500: Player doesn't exist or got unsupported characters in their name (currently spaces are known as such)
