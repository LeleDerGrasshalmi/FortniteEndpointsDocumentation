## Public Key Service - Register Public Key

URL: https://publickey-service-prod.ecbc.live.use1a.on.epicgames.com/publickey/v2/publickey/ <br/>
Method: POST <br/>
Auth Required: Yes (`publickey:public CREATE`)

```json
{
  "algorithm": "ed25519",
  "key": "pnmqMpP/xGvrbXytnmQj2cqtAPKDh1ZoW16HNQBQGSo="
}
```

## Parameters

`algorithm`: `ed25519` (`rsa` is accepted for the same key too) <br/>
`key`: Standard base64 of the raw 32 byte Ed25519 public key

---

*Example Response*

```json
{
  "key": "pnmqMpP/xGvrbXytnmQj2cqtAPKDh1ZoW16HNQBQGSo=",
  "account_id": "5f38c3127c8f44f9b59ae33b095d60b0",
  "key_guid": "64f9d9e8-e2dd-4d2f-b8ce-9c6117b87c50",
  "kid": "20230621",
  "expiration": "2025-05-15T12:15:07.240454571Z",
  "jwt": "eyJhbGciOiJFZERTQSIsInR5cCI6IkpXVCJ9.eyJhY2NvdW50X2lkIjoiNWYzOGMzMTI3YzhmNDRmOWI1OWFlMzNiMDk1ZDYwYjAiLCJnZW5lcmF0ZWQiOjE3NDIxMjczMDcsImtleV9ndWlkIjoiNjRmOWQ5ZTgtZTJkZC00ZDJmLWI4Y2UtOWM2MTE3Yjg3YzUwIiwia2lkIjoiMjAyMzA2MjEiLCJrZXkiOiJwbm1xTXBQL3hHdnJiWHl0bm1RajJjcXRBUEtEaDFab1cxNkhOUUJRR1NvPSIsImV4cGlyYXRpb24iOiIyMDI1LTA1LTE1VDEyOjE1OjA3LjI0MDQ1NDU3MVoiLCJ0eXBlIjoibGVnYWN5In0.YElCnrRM0y8L0gfz0vh7Awf9qLj1B0Sqq9EmEE555cGViSG2ST1k_yby1uKUx1Po9tFDRhj2_bc41Q0eqxsQAg",
  "type": "legacy"
}
```

`jwt` is an EdDSA JWT whose payload holds the same fields (`account_id`, `generated`, `key_guid`, `kid`, `key`, `expiration`, `type`). The `kid` is in the payload, not the header, and matches a key from [Signing Keys](./SigningKeys.md).
