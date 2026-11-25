## Fortnite Website - Discovery Submission

URL: https://fortnite.com/en-US/api/creative-submission-form/submit <br/>
Method: POST <br/>
Auth Required: Yes

```json
{
  "image": false,
  "trailer": false,
  "payload": {
    "submissionIdentifier": "",
    "submissionType": "",
    "islandCode": "",
    "islandType": "",
    "islandVersion": 1,
    "islandTitle": "",
    "islandDescription": "",
    "maxPlayerCount": 1,
    "gameGenre": ""
  }
}
```

## Parameters

`image`: Can be set to true <br/>
`trailer`: Can be set to true <br/>
`payload.submissionIdentifier`: The submission GUID. <br/>
`payload.submissionType`: Can be left empty. Its meaning is undocumented. <br/>
`payload.islandCode`: Island code <br/>
`payload.islandType`: Plot type, ex: CreativePlot:creativeroyaleplot <br/>
`payload.islandVersion`: Island version <br/>
`payload.islandTitle`: Island name <br/>
`payload.islandDescription`: Island description <br/>
`payload.maxPlayerCount`: Amount of players island supports <br/>
`payload.gameGenre`: Main island tag

---

*Example Response*

No example response or status is documented.
