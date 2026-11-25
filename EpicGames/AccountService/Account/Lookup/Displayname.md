## Account Service - Lookup by Display Name

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/displayName/:displayName <br/>
Method: GET <br/>
Auth Required: Yes (`account:public:account READ`)

## Path Parameters

`displayName`: The Display Name to search for

---

*Example Response*

```json
{
  "id": "94b1569506b04f9f8557af611e8c5e47",
  "displayName": "lele stw moment",
  "externalAuths": {}
}
```
