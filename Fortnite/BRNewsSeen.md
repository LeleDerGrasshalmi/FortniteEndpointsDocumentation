## Fortnite - Mark BR News seen

URL: https://prm-dialogue-public-api-prod.edea.live.use1a.on.epicgames.com/api/v1/fortnite-br/surfaces/motd/interactions \
Method: POST \
Auth Required: Yes `(eg1)`

## Body

```js
{
  "sessionId": "XXX", // the sessions id (can be grabbed from verify token api)
  "sessionStartTimestamp": "", // ISO Start Date of the session
  "sessionEndTimestamp": "", // ISO End Date of the Session (current date)
  "events": [
    {
      "type": "view",
      "count": 1, // how often the news got viewedd
      "contentId": "", // the news content id (e.g. 4cdea2e5-d91c-467c-beb0-7ac8cf3daee6)
      "tcId": "", // the news tc id (e.g. 7e4b94ca-ead8-4e44-a578-89cb5f3c2bbe)
      "timestamp": "" // ISO Date, when the news got viewed
    }
  ]
}
```
