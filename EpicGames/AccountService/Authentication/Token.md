## Account Service - Auth: Token

URL: https://account-public-service-prod.ol.epicgames.com/account/api/oauth/token \
Method: POST \
Auth Required: Yes, Basic Auth of the Client Id & Client Secret

## Headers

`Content-Type`: application/x-www-form-urlencoded

## Body

`grant_type`: see [Grants and their required fields](./GrantTypes/) \
`includePerms`: boolean (optional), if the Permissions for the Session should be included (optional) \
`token_type`: (optional) see below

| token_type | Allowed | Description              |
| ---------- | ------- | ------------------------ |
| `*`        |   ✅    | 16 Bytes as hex, Default |
| `eg1`      |   ✅    | Json Web Token           |
| `ep1`      |         |                          |
| `epic_id`  |         |                          |
| `id_token` |         |                          |

<br/>

## Example Request

- `refresh_token` (Request grabbed from EGL Startup)

  ```http
  POST https://account-public-service-prod.ol.epicgames.com/account/api/oauth/token HTTP/1.1
  Host: account-public-service-prod03.ol.epicgames.com
  User-Agent: UELauncher/14.5.0-23755863+++Portal+Release-Live Windows/10.0.19044.1.768.64bit
  Content-Type: application/x-www-form-urlencoded
  Authorization: basic MzRhMDJjZjhmNDQxNGUyOWIxNTkyMTg3NmRhMzZmOWE6ZGFhZmJjY2M3Mzc3NDUwMzlkZmZlNTNkOTRmYzc2Y2Y=

  grant_type=refresh_token&refresh_token=XYZ&token_type=eg1
  ```
