## Account Service - Auth Grant: authorization_code

Login using an Authorization Code (Used for Web Logins). <br/>
You may wanna check out how to get such a code [here](../../../Web/Id/Auth/AuthorizationCode.md).

### Body

`code`: The code you just created <br/>
`code_verifier`: The PKCE code verifier used to generate the authorization code (if any)
