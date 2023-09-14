# Get News

URL: https://sac.epicgames.com/api/get-news \
Method: GET \
Auth Required: Yes

## Query Parameters

`locale`: Optional Content language, e.g. `de`, `en-US`

---

_Example Response (shortened)_

```json
{
  "data": [
    {
      "trending": false,
      "trendingImage": "https://cdn2.unrealengine.com/motd-1920x1080---noqr-1920x1080-acf2c7b797e6.jpg",
      "sticky": false,
      "short": "Reboot-A-Friend",
      "title": "REBOOT A FRIEND: PLAY TOGETHER, EARN TOGETHER!",
      "link": "https://rebootafriend.fortnite.com/",
      "_templateName": "blogLink",
      "id": "1604ad81-f2de-4629-8ce0-bf4033ab5d80",
      "date": "2021-04-06T19:31:36.694Z",
      "externalLink": "https://rebootafriend.fortnite.com/",
      "slug": "reboot-a-friend-launch",
      "url": "/en-US/news/reboot-a-friend-launch",
      "urlPattern": "/news/reboot-a-friend-launch"
    }
  ],
  "success": true
}
```
