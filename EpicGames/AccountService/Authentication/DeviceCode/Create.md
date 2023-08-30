## Account Service - Auth: Create Device Code

URL: https://account-public-service-prod.ol.epicgames.com/account/api/oauth/deviceAuthorization \
Method: POST \
Auth Required: Yes (client_credentials)

---

_Example Response_

```json
{
  "user_code": "VFSBBW9W",
  "device_code": "VjdNNFJSQ0ZHU1pOWU5HQlhZREJCVlZGNkNaMk1KR0dYRkdaUllOOFRKOTlCWU5UUFBOQk1aUExCU1dTUlhIVEdEOUM0NDY5SzJWUFJSVjlWTk1CS0xQTDc4UUJUSEJGWkZUOUw4U1RDUVQ5U0JaVzdEMkRRSFlNSkpKTEhZTDIuVkZTQkJXOVc=",
  "verification_uri": "https://www.epicgames.com/activate",
  "verification_uri_complete": "https://www.epicgames.com/activate?userCode=VFSBBW9W",
  "prompt": "login",
  "expires_in": 600,
  "interval": 10,
  "client_id": "98f7e42c2e3a4f86a74eb43fbb41ed39"
}
```
