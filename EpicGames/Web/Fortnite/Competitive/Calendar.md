## Fortnite Website - Competitive Calendar

URL: https://www.fortnite.com/competitive/en-US/api/calendar \
Method: POST \
Auth Required: No

---

_Example Response (shortened)_

```json
{
  "eventsData": [
    {
      "eventId": "epicgames_ShareTheLove_Placement_Solo_ASIA",
      "regions": ["ASIA"],
      "platforms": [],
      "displayDataId": "stl_placements_solo",
      "announcementTime": "2019-02-08T08:00:00Z",
      "beginTime": "2019-02-09T05:00:00Z",
      "endTime": "2019-02-10T12:00:00Z",
      "eventWindows": [
        {
          "eventWindowId": "ShareTheLove_Placement_Solo_ASIA_Event1",
          "metadata": {},
          "beginTime": "2019-02-09T05:00:00Z",
          "endTime": "2019-02-09T08:00:00Z",
          "requireAllTokens": [],
          "requireAnyTokens": [],
          "requireNoneTokensCaller": [],
          "associatedEventId": "epicgames_ShareTheLove_Placement_Solo_ASIA"
        }
      ],
      "cmsData": {
        "title_line_1": "SHARE THE LOVE",
        "title_line_2": "PLACEMENT SERIES",
        "details_description": "This event will determine initial placement into divisions for the 'Share The Love Series'.  Champion Division - Top 1000 players, Contender Division - Top 3%, Prospect Division - Top 20%. ",
        "poster_front_image": "https://cdn2.unrealengine.com/Fortnite/fortnite-game/tournaments/StLS_Placements_Solo_Front-750x1080-894297bc807f8690702a11edfe1b9f767bb3cd4b.jpg"
      }
    }
  ],
  "playerInfo": null
}
```
