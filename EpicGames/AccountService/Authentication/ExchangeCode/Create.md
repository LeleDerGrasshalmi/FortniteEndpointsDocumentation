## Account Service - Auth: Create Exchange Code

URL: https://account-public-service-prod.ol.epicgames.com/account/api/oauth/exchange \
Method: GET \
Auth Required: Yes (`account:oauth:exchangeTokenCode CREATE`)

### Query Parameters

`consumingClientId`: (optional), the id of the client that should redeem the exchange code <br/>
`codeChallenge`: (optional), a PKCE code challenge <br/>
`codeChallengeMethod`: (optional), the method used to generate the code challenge (`S256` or `plain`)

---

_Example Response (without `consumingClientId`)_

```json
{
  "expiresInSeconds": 299,
  "code": "2c1ef780393741d88a3c9c85423baadb",
  "creatingClientId": "3446cd72694c4a4485d81b77adbb2141"
}
```

_Example Response (with `consumingClientId`)_

```json
{
  "expiresInSeconds": 300,
  "code": "1ab2cdf8486540e6b60e7493891e85eb",
  "creatingClientId": "3446cd72694c4a4485d81b77adbb2141",
  "consumingClientId": "34a02cf8f4414e29b15921876da36f9a"
}
```
