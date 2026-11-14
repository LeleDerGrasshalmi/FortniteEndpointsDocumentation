## Public Key Service - Register Public Key

URL: https://publickey-service-prod.ecbc.live.use1a.on.epicgames.com/publickey/v2/publickey/ \
Method: POST \
Auth Required: Yes (Account Auth)

```json
{
  "algorithm": "ed25519",
  "key": "KjiNzdIo9qri4fFyUm0u7zYV00jgNYjFxWgYkrdVH/w="
}
```

## Parameters

`algorithm`: `ed25519` (`rsa` is accepted for the same key too) <br/>
`key`: Standard base64 of the raw 32 byte Ed25519 public key

---

_Example Response_

```json
{
  "key": "KjiNzdIo9qri4fFyUm0u7zYV00jgNYjFxWgYkrdVH/w=",
  "account_id": "94b1569506b04f9f8557af611e8c5e47",
  "key_guid": "9f3c2a71-5e84-4b0d-a6c9-1d7e2f8b4a30",
  "kid": "20230621",
  "expiration": "2026-12-13T16:53:45.412484099Z",
  "jwt": "REDACTED",
  "type": "legacy"
}
```

`jwt` is an EdDSA JWT whose payload holds the same fields (`account_id`, `generated`, `key_guid`, `kid`, `key`, `expiration`, `type`). The `kid` is in the payload, not the header, and matches a key from [Signing Keys](./SigningKeys.md).
