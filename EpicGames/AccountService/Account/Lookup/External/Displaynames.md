## Account Service - Lookup by External Display Name (Bulk)

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/lookup/externalDisplayName \
Method: POST \
Auth Required: Yes (`account:public:account:lookup:externalDisplayName:{externalAuthType} READ`)

`Max 100 Account Lookups per request.`

```json
{
  "authType": "psn",
  "displayNames": ["LeleSaysHi"]
}
```

## Parameters

`authType`: See via [External Auth Readme](../../ExternalAuth/README.md) <br/>
`displayNames`: Displaynames, need to be the exact case
