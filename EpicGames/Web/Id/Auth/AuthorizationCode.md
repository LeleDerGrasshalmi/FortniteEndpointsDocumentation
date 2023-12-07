## Id Web - Create Authorization Code

URL: https://www.epicgames.com/id/api/redirect \
Method: GET \
Auth Required: Yes

## Query Parameters

`clientId`: The Id of the Client that the Authorization Code should be issued for <br/>
`responseType`: Must be `code` <br/>
`exchangeCode`: (optional), a valid exchange code (the usage is unknown) <br/>
`codeChallenge`: (optional), a PKCE code challenge <br/>
`codeChallengeMethod`: (optional), the method used to generate the code challenge (`S256` or `plain`) <br/>
`scope`: (optional), a space seperated list of scopes <br/>
`redirectUrl`: (optional), Automaticly redirect to that URL with the `code` Query being set to the created Authorization Code

---

_Example Response_

```json
{
  "redirectUrl": "https://accounts.epicgames.com/fnauth?code=c5a0b794bd5b4fb39d5d7b9e32b43f12",
  "authorizationCode": "c5a0b794bd5b4fb39d5d7b9e32b43f12",
  "exchangeCode": null
  "sid": null
}
```
