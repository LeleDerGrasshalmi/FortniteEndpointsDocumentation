## Public Key Service - Signing Keys

URL: https://publickey-service-prod.ecbc.live.use1a.on.epicgames.com/publickey/v2/publickey/signing \
Method: GET \
Auth Required: Yes (Account Auth)

---

_Example Response_

```json
{
  "keys": [
    {
      "crv": "P-256",
      "kid": "1",
      "kty": "EC",
      "x": "Z1wgnXPU2cGuQ7gmt8ErapzyH4iFOcq6zgM1I5hnT9Y",
      "y": "7Ckc161-P7jkbMtSjToMXrR-3s-O450w_W899513d34"
    },
    {
      "crv": "Ed25519",
      "kid": "20230621",
      "kty": "OKP",
      "x": "zsas3J1p4mt_5V6LdnA1BEqwvFtvG9nYtERMVOEfLoc"
    }
  ]
}
```

The Ed25519 key verifies the `jwt` returned by [Register Public Key](./Register.md) (signature over `header.payload`).
