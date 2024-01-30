## Persona Service - Lookup by Display Name

URL: https://persona-public-service-prod06.ol.epicgames.com/persona/api/public/account/lookup \
Method: GET \
Auth Required: Yes (`persona:account:lookup READ`)

## Query Parameters

`q`: The account's DisplayName to lookup (q stands for Query)

---

_Example Response_

```json
{
  "id": "94b1569506b04f9f8557af611e8c5e47",
  "displayName": "lele stw moment"
}
```
