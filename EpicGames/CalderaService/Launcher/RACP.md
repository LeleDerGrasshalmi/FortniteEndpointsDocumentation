## Caldera Service - Request Anti Cheat Provider (RACP)

URL: https://caldera-service-prod.ecosec.on.epicgames.com/caldera/api/v1/launcher/racp \
Method: POST \
Auth Required: No

```json
{
  "account_id": "",
  "exchange_code": "",
  "test_mode": false,
  "epic_app": "",
  "nvidia": false,
  "luna": false
}
```

## Parameters

`account_id`: Your Account Id <br/>
`exchange_code`: Your [Exchange Code](../../AccountService/Authentication/ExchangeCode/Create.md) <br/>
`test_mode`: Unknown, just leave it false <br/>
`epic_app`: The Game you want to launch e.g. `fortnite` <br/>
`nvidia`: Used for the Nvidia Gefore Cloud-Gaming, if this is true **all** other parameters can be ignored <br/>
`luna`: Used for the Amazon Luna Cloud-Gaming, if this is true **all** other parameters can be ignored

---

Example Response (NVIDIA Mode)

```json
{
  "provider": "EasyAntiCheat",
  "jwt": "eyJhbGciOiJFUzI1NiIsInR5cCI6IkpXVCJ9.eyJhY2NvdW50X2lkIjoiXHUwMDNjbnZpZGlhXHUwMDNlIiwiZ2VuZXJhdGVkIjoxNjgzMDQ3OTk4LCJjYWxkZXJhR3VpZCI6IjYxNDIzMjQxLWE4MWYtNGEzYS05YjM4LTUxNjVmNWJlYmMzOSIsImFjUHJvdmlkZXIiOiJFYXN5QW50aUNoZWF0Iiwibm90ZXMiOiI4MzFhNDkzYy1kYzYxLTQ0NTgtYjI1YS05OGYwZjMxMTUzMTgiLCJmYWxsYmFjayI6ZmFsc2V9.OHZR7bElxV1RmoQaXPTPGcv6TgNBwQ7GI2so_JSlHG8LXlV5sBlfazWlV3WjxsT7V2T6iL0E1YnZD6J6bQMs0A"
}
```
