## Account Service - Auth: Continuation Token Info

URL: https://account-public-service-prod.ol.epicgames.com/account/api/oauth/continuationToken/:continuationToken \
Method: GET \
Auth Required: Yes (`account:oauth:continuationToken READ`)

## Path Parameters

`continuationToken`: 16 Bytes in hex token

_Example Response (Any Corrective Action)_

```json
{
  "tokenId": "cf98b44dfe4641778cca075bc1319ccb",
  "shortTokenId": "cb5133c6",
  "clientId": "xyza7891ov4bjltiTDG4lfbFq7aPJjm1",
  "accountId": "8b0a23cb43af46cb972806f4025a9cba",
  "scopes": [
    "email"
  ],
  "correctiveAction": "SCOPE_CONSENT",
  "ageGateRequired": true,
  "acr": "urn:epic:loa:aal1"
}
```

_Example Response (With `EXTERNAL_AUTH_NOT_FOUND` corrective action)_

```json
{
    "tokenId": "cf98b44dfe4641778cca075bc1319ccb",
    "shortTokenId": "cb5133c6",
    "clientId": "xyza7891p5D7s9R6Gm6moTHWGloerp7B",
    "scopes": [],
    "platformType": "nintendo",
    "externalAuthId": "lp1_00QIU7B6WPKJJXM56TXIDBVY2FPE",
    "externalAuthEnv": "lp1",
    "correctiveAction": "EXTERNAL_AUTH_NOT_FOUND",
    "ageGateRequired": true,
    "acr": "urn:epic:loa:aal1"
}
```
