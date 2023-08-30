## Id Web - Create Authorization Code

URL: https://www.epicgames.com/id/api/redirect \
Method: GET \
Auth Required: Yes

## Query Parameters

`clientId`: the clients Id you want to create the Code for \
`responseType`: must be `code` \
`codeChallenge`: (optional), a PKCE code challenge \
`codeChallengeMethod`: (optional), the method used to generate the code challenge (`S256` or `plain`)
`scope`: (optional), a space seperated list of scopes

---

_Example Response_

```json
{
  "redirectUrl": "https://accounts.epicgames.com/fnauth?code=c5a0b794bd5b4fb39d5d7b9e32b43f12",
  "authorizationCode": "c5a0b794bd5b4fb39d5d7b9e32b43f12",
  "sid": null
}
```
