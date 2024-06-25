## Account Service - Auth: Token

If you need help check out the [getting started guide](./README.md#getting-started)

URL: https://account-public-service-prod.ol.epicgames.com/account/api/oauth/token \
Method: POST \
Auth Required: Yes (Basic Authentication where the username is the Client Id and the password is the Client Secret)

## Headers

`Content-Type`: application/x-www-form-urlencoded <br/>
`X-Epic-Device-ID`: A random value used to identify a device.

## Parameters

`grant_type`: see [Grants and their required fields](./GrantTypes/) <br/>
`includePerms`: boolean (optional), if the Permissions for the Session should be included <br/>
`deployment_id`: (optional) an EOS [deployment id](https://dev.epicgames.com/docs/dev-portal/product-management#deployments) <br/>
`token_type`: (optional) see below

| Token Type | Allowed | Description                                                                                                                                          |
| ---------- | ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| `*`        | ✅      | A 16 byte hexadecimal session id. (default)                                                                                                          |
| `eg1`      | ✅      | A signed jwt prefixed with `eg1~`.                                                                                                                   |
| `ep1`      |         | An encrypted jwt prefixed with `ep1~`. Can be gotten with the external_auth grant type or from the [PlatformToken API](../Account/PlatformToken.md). |
| `epic_id`  |         | A signed jwt used for EOS. Can be gotten from [EOS Auth Web APIs](https://dev.epicgames.com/docs/web-api-ref/authentication).                        |
| `id_token` |         | An OpenID Connect token. Can be gotten from [EOS Auth Web APIs](https://dev.epicgames.com/docs/web-api-ref/authentication) with the openid scope.    |

<br/>

## Example Request

- `refresh_token` (Request grabbed from EGL Startup)

  ```http
  POST /account/api/oauth/token HTTP/1.1
  Host: account-public-service-prod.ol.epicgames.com
  User-Agent: UELauncher/14.5.0-23755863+++Portal+Release-Live Windows/10.0.19044.1.768.64bit
  Content-Type: application/x-www-form-urlencoded
  Authorization: basic MzRhMDJjZjhmNDQxNGUyOWIxNTkyMTg3NmRhMzZmOWE6ZGFhZmJjY2M3Mzc3NDUwMzlkZmZlNTNkOTRmYzc2Y2Y=

  grant_type=refresh_token&refresh_token=XYZ&token_type=eg1
  ```

---

_Example Response (`client_credentials` Grant)_

```json
{
  "access_token": "41ff4aeaede44f62b81a57688b0b6ef3",
  "expires_in": 14400,
  "expires_at": "2023-08-30T20:32:21.466Z",
  "token_type": "bearer",
  "client_id": "ec684b8c687f479fadea3cb2ad83f5c6",
  "internal_client": true,
  "client_service": "prod-fn",
  "product_id": "prod-fn",
  "application_id": "fghi4567FNFBKFz3E4TROb0bmPS8h1GW"
}
```

_Example Response (`exchange_code` Grant)_

```json
{
  "access_token": "065981d58ba642e7ac6ef7d6c4ed15b2",
  "expires_in": 7200,
  "expires_at": "2023-08-30T18:29:11.892Z",
  "token_type": "bearer",
  "refresh_token": "4f665dd625f146bf8d6a57f8af327aaf",
  "refresh_expires": 28800,
  "refresh_expires_at": "2023-08-31T00:29:11.893Z",
  "account_id": "94b1569506b04f9f8557af611e8c5e47",
  "client_id": "ec684b8c687f479fadea3cb2ad83f5c6",
  "internal_client": true,
  "client_service": "prod-fn",
  "displayName": "lele stw moment",
  "app": "prod-fn",
  "in_app_id": "94b1569506b04f9f8557af611e8c5e47",
  "product_id": "prod-fn",
  "application_id": "fghi4567FNFBKFz3E4TROb0bmPS8h1GW"
}
```
