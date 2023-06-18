## FN - Discovery Service: Check Links Favorite Status

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v1/links/favorites/:accountId/check \
Method: POST \
Auth Required: Yes (`discovery:{accountId}:links:favorite READ`)

```json
{
  "linkCodes": ["1111-1111-1111", "6276-3568-1807"]
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`linkCodes`: The Mnemonics to check

---

_Example Response_

Returns all links that `are already favorited`, so in the example I have `1111-1111-1111` favorited and `6276-3568-1807` is not favorited.

```json
{
  "results": [
    {
      "playerId": "94b1569506b04f9f8557af611e8c5e47",
      "linkCode": "1111-1111-1111",
      "linkType": "Creative:Island",
      "sortDate": "2023-05-30T17:52:16.271Z",
      "pagingDate": "2023-05-30T17:52:16.271Z"
    }
  ],
  "hasMore": false
}
```
