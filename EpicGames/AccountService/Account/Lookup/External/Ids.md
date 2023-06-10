## Account Service - Lookup by External Id (Bulk)

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/lookup/externalId \
Method: POST \
Auth Required: Yes (`account:public:account:lookup:externalId READ`)

```json
{
  "authType": "nintendo",
  "ids": ["lp1_e7b6e8e2e07fab26"]
}
```

## Parameters

`authType`: See via [External Auth Readme](../../ExternalAuth/README.md) <br/>
`ids`: this is for most external accounts some string number **[Max 100 per Request]**

---

_Example Response_

```json
{
  "lp1_e7b6e8e2e07fab26": {
    "accountId": "020b5d9042174a7692f20db8e23b84d1",
    "type": "nintendo",
    "externalAuthId": "lp1_e7b6e8e2e07fab26",
    "externalAuthIdType": "nintendo_id",
    "authIds": [
      {
        "id": "lp1_e7b6e8e2e07fab26",
        "type": "nintendo_id"
      }
    ]
  }
}
```
