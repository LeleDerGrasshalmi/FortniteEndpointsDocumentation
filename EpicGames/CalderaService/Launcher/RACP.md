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
  "nvidia": false
}
```

## Parameters

`account_id`: Your Account Id <br/>
`exchange_code`: Your [Exchange Code](../../AccountService/Authentication/ExchangeCode/Create.md) <br/>
`test_mode`: Unknown, just leave it false <br/>
`epic_app`: The Game you want to launch e.g. `fortnite` <br/>
`nvidia`: If this is true **all** other parameters can be ignored
