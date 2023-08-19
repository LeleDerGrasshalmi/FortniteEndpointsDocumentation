## Account Service - EpicId Auth: Token Info

URL: https://account-public-service-prod.ol.epicgames.com/account/api/epicid/v1/oauth/tokenInfo \
Method: POST \
Auth Required: Yes (In Body, not in the Authorization Header)

## Headers

`Content-Type`: application/x-www-form-urlencoded

<br/>

```
token=abc
```

## Parameters

`token`: Your Bearer Token

---

_Example Response (Valid)_

```json
{
  "active": true,
  "token_type": "bearer",
  "expires_in": 14385,
  "expires_at": "2023-06-10T23:20:01.156Z",
  "client_id": "ec684b8c687f479fadea3cb2ad83f5c6",
  "application_id": "fghi4567FNFBKFz3E4TROb0bmPS8h1GW"
}
```

_Example Response (Not Active / Invalid)_

```json
{
  "active": false
}
```
