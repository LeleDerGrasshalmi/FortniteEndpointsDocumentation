## PRM Dialog Service - Fortnite BR: Dynamic MOTD Interactions

URL: https://prm-dialogue-public-api-prod.edea.live.use1a.on.epicgames.com/api/v1/fortnite-br/surfaces/dmotd/interactions \
Method: POST \
Auth Required: Yes (Account - `eg1`)

```json
{
  "sessionId": "DFA9F76E48DF551857C6F9ACEE7A2FE2",
  "sessionStartTimestamp": "2023-10-30T17:19:04.591Z",
  "sessionEndTimestamp": "2023-10-30T17:20:55.356Z",
  "events": [
    {
      "type": "impression",
      "count": 4,
      "timestamp": "2023-10-30T17:19:09.441Z",
      "lastTimestamp": "2023-10-30T17:20:42.300Z",
      "contentId": "7b1f8ed0-21cc-43e5-b0c8-e45b7537785d"
    },
    {
      "type": "impression",
      "count": 3,
      "timestamp": "2023-10-30T17:19:20.640Z",
      "lastTimestamp": "2023-10-30T17:20:26.285Z",
      "contentId": "2c068b75-a921-4008-9db9-86213e95167c"
    },
    {
      "type": "impression",
      "count": 3,
      "timestamp": "2023-10-30T17:19:25.977Z",
      "lastTimestamp": "2023-10-30T17:20:31.625Z",
      "contentId": "eef866a8-8bd7-492e-89ed-a3310d073586"
    },
    {
      "type": "impression",
      "count": 3,
      "timestamp": "2023-10-30T17:19:31.311Z",
      "lastTimestamp": "2023-10-30T17:20:36.959Z",
      "contentId": "365092b9-3f6d-4aff-a439-416bf66399df"
    },
    {
      "type": "impression",
      "count": 3,
      "timestamp": "2023-10-30T17:19:42.013Z",
      "lastTimestamp": "2023-10-30T17:20:47.575Z",
      "contentId": "43cd2eeb-60dc-49d7-8779-4bb422c11f85"
    }
  ]
}
```

## Parameters

`sessionId`: Can be extracted from the JWT (`jti`), or grabbed from [Verifying the Token](../../AccountService/Authentication/Verify.md) <br/>
`sessionStartTimestamp`: When your Session started <br/>
`sessionEndTimestamp`: When your Session ends (current timestamp) <br/>
`events[].type`: Only known type is 'impression' <br/>
`events[].count`: How often you have viewed the MOTD <br/>
`events[].timestamp`: When the content got first viewed <br/>
`events[].lastTimestamp`: When the last Interaction with that content was (current timestamp) <br/>
`events[].contentId`: Related to the [Content](./DynamicMOTD.md)'s Item <br/>

---

_Example Response_

`Status 200` (But no Content)
