## Party Service V2 - Join

URL: https://api.epicgames.dev/epic/party/internal/v2/parties/:partyId/members/:accountId/join \
Method: POST \
Auth Required: Yes (Account Auth)

```json
{
  "connection": {
    "id": "6b4e20fffe8a1d57-00000001-05a3e9c1-7d2f4b6a8c0e1f35-2c9a7e4b",
    "deployment_id": "_",
    "meta": {
      "osName": "Windows",
      "platformName": "egs",
      "productName": "Epic Games Launcher"
    }
  }
}
```

## Path Parameters

`partyId`: The Party ID <br/>
`accountId`: Your AccountId

## Parameters

`connection.id`: Your Connection ID (EOS Connect Stomp) <br/>
`connection.deployment_id`: The deployment id, e.g. `_` <br/>
`connection.meta`: Connection metadata

---

_Example Response_

```json
{
  "status": "JOINED",
  "party_id": "2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f"
}
```
