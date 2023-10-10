## PRM Dialog Service - Fortnite BR: MOTD Interactions

URL: https://prm-dialogue-public-api-prod.edea.live.use1a.on.epicgames.com/api/v1/fortnite-br/surfaces/motd/interactions \
Method: POST \
Auth Required: Yes (Account - `eg1`)

```json
{
  "sessionId": "97d4bb5fe94649f484ac63c120efa056",
  "sessionStartTimestamp": "2023-01-31T21:46:13.297Z",
  "sessionEndTimestamp": "2023-01-31T21:47:13.297Z",
  "events": [
    {
      "type": "view",
      "count": 1,
      "contentId": "546fe8ae-99ea-47fe-bd05-68a645988a23",
      "tcId": "931018bb-4ded-4b72-acfa-d8a4b39feb8d",
      "timestamp": "2023-01-31T21:47:13.297Z"
    }
  ]
}
```

## Parameters

`sessionId`: Can be extracted from the JWT (`jti`), or grabbed from [Verifying the Token](../../AccountService/Authentication/Verify.md) <br/>
`sessionStartTimestamp`: When your Session started <br/>
`sessionEndTimestamp`: When your Session ends (current timestamp) <br/>
`events[].type`: Only known type is 'view' <br/>
`events[].count`: How often you have viewed the MOTD <br/>
`events[].contentId`: Related to the [MOTD](./MOTD.md)'s Item <br/>
`events[].tcId`: Related to the [MOTD](./MOTD.md)'s Item <br/>
`events[].timestamp`: When the MOTD Item got viewed (likely current Date)

---

_Example Response_

`Status 200` (But no Content)
