## Tag Management Service - Tags List

> **This endpoint is no longer available.**

URL: https://tag-management-public-service-prod.identity.live.on.epicgames.com/api/v1/public/tags <br/>
Method: GET <br/>
Auth Required: Yes (Account Auth)

## Query Parameters

`count`: (optional), the amount of tags returned, defaults to 20 (can be any value, but must be within the range of a int32) <br/>
`cursor`: (optional), used for paging, returned in the response for the next request

---

*Example Response (shortened)*

```json
{
  "tags": [
    {
      "id": "d9e00ab236c343268ebc1fe479b960e6",
      "name": "BR - Duos",
      "types": ["Game Modes"],
      "locale": "en-US",
      "defaultLocaleName": "BR - Duos"
    }
  ],
  "cursor": "dGFnczppbmRleGVkOjIwOjIw"
}
```
