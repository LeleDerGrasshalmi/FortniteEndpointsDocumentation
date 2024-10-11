## PRM Dialog Service - Interactions

URL: https://prm-dialogue-public-api-prod.edea.live.use1a.on.epicgames.com/api/v1/fortnite-br/interactions \
Method: POST \
Auth Required: Yes (Account - `eg1`)

```json
{
  "events": {
    "motd": [
      {
        "type": "impression",
        "trackingId": "56c5772d-cc06-4f6e-ba78-a95a85bd5c94",
        "tag": "Product.STW",
        "count": 1,
        "timestamp": "2024-08-31T09:28:07.921Z",
        "lastTimestamp": "2024-08-31T09:28:07.921Z"
      }
    ]
  }
}
```

## Parameters

`events.motd`: Array of MOTDs data <br/>
`events.motd[].type`: Only known type is 'impression' <br/>
`events.motd[].trackingId`: Related to the MOTD's Item <br/>
`events.motd[].tag`: In which context the interaction occured <br/>
`events.motd[].count`: How often you have viewed the MOTD <br/>
`events.motd[].timestamp`: When the content got first viewed <br/>
`events.motd[].lastTimestamp`: When the last Interaction with that content was (current timestamp)

---

_Example Response_

`Status 200` (But no Content)
