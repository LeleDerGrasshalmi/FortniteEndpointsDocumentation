## Fortnite Website - Discovery Submission

URL: https://fortnite.com/en-US/api/creative-submission-form/submit \
Method: POST \
Auth Required: Yes

```js
{
  "image": false, // can be set to true
  "trailer": false, // can be set to true
  "payload": {
    "submissionIdentifier": "", // submission-guid
    "submissionType": "", // idk can be left empty
    "islandCode": "", // island code
    "islandType": "", // plot type, ex: CreativePlot:creativeroyaleplot
    "islandVersion": 1, // island version
    "islandTitle": "", // island name
    "islandDescription": "", // island description
    "maxPlayerCount": 1, // amount of players island supports
    "gameGenre": "" // main island tag
  }
}
```
