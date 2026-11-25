## Events Service - Player Tokens

URL: https://events-public-service-live.ol.epicgames.com/api/v1/players/:gameId/tokens <br/>
Method: GET <br/>
Auth Required: Yes

## Path Parameters

`gameId`: Fortnite

## Query Parameters

`teamAccountIds`: Account Ids seperated by a comma `,`

---

*Example Response*

```json
{
  "accounts": [
    {
      "accountId": "94b1569506b04f9f8557af611e8c5e47",
      "tokens": [
        "Arena_S24_Division1",
        "GroupIdentity_GeoIdentity_Germany",
        "GroupIdentity_Lele_is_Cool"
      ]
    }
  ]
}
```
