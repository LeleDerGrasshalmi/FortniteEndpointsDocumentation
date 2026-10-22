## Presence Service - Set Presence (Internal)

URL: https://api.epicgames.dev/epic/presence/internal/v1/:namespace/:accountId/presence/:connectionId \
Method: POST \
Auth Required: Yes (Account Auth)

## Headers

`Content-Type`: `application/json` <br/>
`X-HTTP-Method-Override`: `PATCH`

<br/>

```json
{
  "status": "online",
  "party": {
    "id": "2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f",
    "type": "INVITE_ONLY",
    "timestamp": "2026-10-14T16:53:45.111Z",
    "memberCount": 1,
    "clientJoinable": true
  },
  "conn": {
    "props": {}
  }
}
```

## Path Parameters

`namespace`: The presence namespace, ex. `_` <br/>
`accountId`: Your AccountId <br/>
`connectionId`: Your Connection ID (EOS Connect Stomp)

## Parameters

`status`: e.g. `online` <br/>
`party`: Your [Party V2](../../PartyService/V2) info, `type` is the party joinability and `timestamp` the party creation date <br/>
`conn.props`: Connection properties

---

_Example Response_

```json
{
  "own": {
    "accountId": "94b1569506b04f9f8557af611e8c5e47",
    "status": "online",
    "perNs": [
      {
        "status": "online",
        "party": {
          "joinable": false,
          "invitable": true
        },
        "ns": "_",
        "conns": [
          {
            "id": "3a9c51fffe7d2e48-00000001-0007c2d4-5b1e9f0a7c3d2b6e-4f8a1c2d",
            "props": {}
          }
        ]
      }
    ]
  }
}
```
