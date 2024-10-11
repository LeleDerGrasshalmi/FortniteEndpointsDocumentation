## PRM Dialog Service - Interactions (Content Hash)

URL: https://prm-dialogue-public-api-prod.edea.live.use1a.on.epicgames.com/api/v1/fortnite-br/interactions/contentHash \
Method: POST \
Auth Required: Yes (Account - `eg1`)

> Removed as of 30.09.2024

```json
{
  "sessionId": "21BED1F74D434A9678C4E584A4CF4257",
  "sessionStartTimestamp": "2023-12-03T10:04:55.306Z",
  "surfaces": [
    {
      "surfaceId": "br-motd",
      "contentMeta": [
        "{\"7a427ff816c8321910c5b6020dd410a4\":[\"0ac665f8-24f4-4ddf-85a4-8557293aba53\"],\"c139b049ff3bd2dc4224b9a0befbc3b5\":[\"8a1e450d-7513-41c9-9289-4af90f985557\"],\"5532ab90cff25c1f66ca1f605cb97d11\":[\"f78c8632-0b86-4698-b204-1bac475c2c6e\"],\"03d5ea4cdbe83ece0fb9255a545fc00f\":[\"f55366b6-fd78-4b06-9ba1-0f8312453f3f\"],\"2d597ddb9dcb097166feebdf2c525bba\":[\"a8ab427d-94c9-4bfc-b06c-24d1d5bb217b\"]}"
      ],
      "events": [
        {
          "contentHash": "7a427ff816c8321910c5b6020dd410a4",
          "type": "impression",
          "count": 1,
          "timestamp": "2023-12-03T10:17:41.387Z",
          "lastTimestamp": "2023-12-03T10:17:41.387Z"
        },
        {
          "contentHash": "2d597ddb9dcb097166feebdf2c525bba",
          "type": "impression",
          "count": 1,
          "timestamp": "2023-12-03T10:17:46.695Z",
          "lastTimestamp": "2023-12-03T10:17:46.695Z"
        }
      ]
    }
  ]
}
```

## Parameters

`sessionId`: Can be extracted from the JWT (`jti`), or grabbed from [Verifying the Token](../AccountService/Authentication/Verify.md) <br/>
`sessionStartTimestamp`: When your Session started <br/>
`sessionEndTimestamp`: When your Session ends (current timestamp) <br/>
`surfaces[].surfaceId`: The SurfaceId that the interaction belongs to (see [Surfaces](README.md#surfaces)) <br/>
`surfaces[].contentMeta`: From the surface MOTD query response <br/>
`surfaces[].events`: Array of MOTDs data <br/>
`surfaces[].events[].contentHash`: Related to the MOTD's Item <br/>
`surfaces[].events[].type`: Only known type is 'impression' <br/>
`surfaces[].events[].count`: How often you have viewed the MOTD <br/>
`surfaces[].events[].timestamp`: When the content got first viewed <br/>
`surfaces[].events[].lastTimestamp`: When the last Interaction with that content was (current timestamp)

---

_Example Response_

`Status 200` (But no Content)
