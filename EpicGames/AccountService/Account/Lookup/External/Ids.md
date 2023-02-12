## Account Service - Lookup by External Id (Bulk)

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/lookup/externalId \
Method: POST \
Auth Required: Yes (`account:public:account:lookup:externalId READ`)

`Max 100 Account Lookups per request.`

```json
{
  "authType": "psn",
  "ids": ["123456789"]
}
```

## Parameters

`authType`: See via [External Auth Readme](../../ExternalAuth/README.md) <br/>
`ids`: this is for most external accounts some string number
