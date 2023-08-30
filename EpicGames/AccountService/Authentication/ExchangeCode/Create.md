## Account Service - Auth: Create Exchange Code

URL: https://account-public-service-prod.ol.epicgames.com/account/api/oauth/exchange \
Method: GET \
Auth Required: Yes (`account:oauth:exchangeTokenCode CREATE`)

### Query Parameters

`consumingClientId`: (optional), the id of the client that should redeem the exchange code \
`codeChallenge`: (optional), a PKCE code challenge \
`codeChallengeMethod`: (optional), the method used to generate the code challenge (`S256` or `plain`)