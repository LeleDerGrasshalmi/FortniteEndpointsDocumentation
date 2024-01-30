# Getting started

Epic Games uses [OAuth2](https://auth0.com/intro-to-iam/what-is-oauth-2) for authentication.

1. In order to authenticate you first need to decide for which client you want to authenticate for. A list of clients can be found [here](./Clients.md) or on https://egs.jaren.wtf, which also allows to search by permission.
2. Now you need to build the [basic auth header](https://developer.mozilla.org/en-US/docs/Web/HTTP/Authentication#basic_authentication_scheme). So you will need to base64 encode the following formatted string `{clientId}:{clientSecret}` (replace the variables). <br/> So for the `fortnitePCGameClient` client this would be`ZWM2ODRiOGM2ODdmNDc5ZmFkZWEzY2IyYWQ4M2Y1YzY6ZTFmMzFjMjExZjI4NDEzMTg2MjYyZDM3YTEzZmM4NGQ=`.
3. Then you need to decide, if you want to authenticate as the client, or as a account. You should remember that many apis require account authentication and possibly also require an eg1 (JWT) access token, which can be gotten with including the `token_type` parameter with the `eg1` value in the token request.

## Client Authentication

When you want to authenticate as a client, you will need to use the [`client_credentials`](./GrantTypes/client_credentials.md) Grant Type.

So this would be an example http request for the `fortnitePCGameClient` client.

```http
POST /account/api/oauth/token HTTP/1.1
Host: account-public-service-prod.ol.epicgames.com
Content-Type: application/x-www-form-urlencoded
Authorization: Basic ZWM2ODRiOGM2ODdmNDc5ZmFkZWEzY2IyYWQ4M2Y1YzY6ZTFmMzFjMjExZjI4NDEzMTg2MjYyZDM3YTEzZmM4NGQ=

grant_type=client_credentials
```

Which will respond with the authentication session.

```json
{
  "access_token": "266e2719635f4a899e94bd19c4422a90",
  "expires_in": 14400,
  "expires_at": "2023-11-12T13:29:34.070Z",
  "token_type": "bearer",
  "client_id": "ec684b8c687f479fadea3cb2ad83f5c6",
  "internal_client": true,
  "client_service": "prod-fn",
  "product_id": "prod-fn",
  "application_id": "fghi4567FNFBKFz3E4TROb0bmPS8h1GW"
}
```

## Account Authentication

When you decide to authenticate as a account, you need to choose the way to authenticate (e.g. external auth like playstation, authorization code, etc.)

Using the authorization code is usually the easiest:

1. Login to epicgames.com
2. Check out the [authorization code creation web api](../../Web/Id/Auth/Redirect.md) docs how to create such a code
3. Send the request to exchange the code for a authentication session

```http
POST /account/api/oauth/token HTTP/1.1
Host: account-public-service-prod.ol.epicgames.com
Content-Type: application/x-www-form-urlencoded
Authorization: Basic ZWM2ODRiOGM2ODdmNDc5ZmFkZWEzY2IyYWQ4M2Y1YzY6ZTFmMzFjMjExZjI4NDEzMTg2MjYyZDM3YTEzZmM4NGQ=

grant_type=authorization_code&code=REPLACE_THIS
```

Which will respond with

```json
{
  "access_token": "7c0aa5ad4721454a81a0f48683715978",
  "expires_in": 7200,
  "expires_at": "2023-11-12T13:06:47.813Z",
  "token_type": "bearer",
  "refresh_token": "a2f033647d414de2bbe04b1c12b5b5ee",
  "refresh_expires": 28800,
  "refresh_expires_at": "2023-11-12T19:06:47.814Z",
  "account_id": "94b1569506b04f9f8557af611e8c5e47",
  "client_id": "ec684b8c687f479fadea3cb2ad83f5c6",
  "internal_client": true,
  "client_service": "prod-fn",
  "scope": ["basic_profile"],
  "displayName": "lele stw moment",
  "app": "prod-fn",
  "in_app_id": "94b1569506b04f9f8557af611e8c5e47",
  "device_id": "63e3b71af76e4fc48841b92c5eb3d69d",
  "product_id": "prod-fn",
  "application_id": "fghi4567FNFBKFz3E4TROb0bmPS8h1GW"
}
```
