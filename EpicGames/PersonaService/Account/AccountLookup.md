## Persona Service - Lookup by Display Name

> **This endpoint is no longer available.** Persona Service shut down on February 19, 2020.

URL: https://persona-public-service-prod06.ol.epicgames.com/persona/api/public/account/lookup <br/>
Method: GET <br/>
Auth Required: Yes (`persona:account:lookup READ`)

## Query Parameters

`q`: The account's DisplayName to lookup (q stands for Query)

---

*Example Response*

```json
{
  "id": "94b1569506b04f9f8557af611e8c5e47",
  "displayName": "lele stw moment"
}
```
