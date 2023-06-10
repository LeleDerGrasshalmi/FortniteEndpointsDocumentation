## Account Service - Lookup by External Display Name (Bulk)

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/lookup/externalDisplayName \
Method: POST \
Auth Required: Yes (`account:public:account:lookup:externalDisplayName:{externalAuthType} READ`)

```json
{
  "authType": "xbl",
  "displayNames": ["jemcer"]
}
```

## Parameters

`authType`: See via [External Auth Readme](../../ExternalAuth/README.md) <br/>
`displayNames`: Displaynames, CaseSensitive **[Max 100 per Request]**

---

_Example Response_

```json
{
  "jemcer": [
    {
      "accountId": "bec13864ce1d44148e04cb82401c4257",
      "type": "xbl",
      "externalAuthIdType": "xuid",
      "externalDisplayName": "jemcer"
    }
  ]
}
```
