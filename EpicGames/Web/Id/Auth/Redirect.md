## Id Web - Redirect

URL: https://www.epicgames.com/id/api/redirect \
Method: GET \
Auth Required: Yes

## Query Parameters

`clientId`: The ID of the client you are redirecting to <br/>
`responseType`: The responseType you want to use (for non-EOS Clients: `code`, `eula_token` for EOS Clients: `code`) <br/>
`provider`: (optional) The external account provider (ex. psn, nintendo, ps5, xbox, vk, apple, lego) <br/>
`state`: (optional) The login state obtained from [here](../CreateOAuthState.md) <br/>
`userCode`: (optional) A valid [User Code](../../../AccountService/Authentication/DeviceCode/Create.md) <br/>
`continuation`: (optional) A valid Continuation Token <br/>
`exchangeCode`: (optional), a valid exchange code (the usage is unknown) <br/>
`codeChallenge`: (optional), a PKCE code challenge <br/>
`codeChallengeMethod`: (optional), the method used to generate the code challenge (`S256` or `plain`) <br/>
`nonce`: (optional) A random value used to associate a request to a token. This value is reflected inside of epic_id tokens and id tokens. <br/>
`scope`: (optional), A space seperated list of scopes <br/>
`eula`: (optional, deprecated), A valid eula ID (ex. `fn`, `tos`) <br/>
`prompt`: (optional), The redirect prompt, (ex. `none`, `login`, `new_session`, `register`, `consent`, `pass_through`, `2nd_domain`, `upgrade`)  <br/>
`redirectUrl`: (optional), The URL to redirect to

---

_Example Response (responseType=code)_

```json
{
  "redirectUrl": "https://accounts.epicgames.com/fnauth?code=c5a0b794bd5b4fb39d5d7b9e32b43f12",
  "authorizationCode": "c5a0b794bd5b4fb39d5d7b9e32b43f12",
  "exchangeCode": null
  "sid": null
}
```
_Example Response (responseType=eula_token or no responseType specified)_

```json
{
   "redirectUrl":"https://epicgames.com/account/personal",
   "authorizationCode":null,
   "exchangeCode":null,
   "sid":"54719c4b12444f6695f4c2aab2fced99"
}
```
