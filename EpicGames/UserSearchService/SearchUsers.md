## User-Search Service - Search Users

URL: https://user-search-service-prod.ol.epicgames.com/api/v1/search/:accountId \
Method: GET \
Auth Required: Yes (`social:search:{accountId} READ`)

## Path Parameters

`accountId`: Your Account Id

## Query Parameters

`platform`: (required), known valid values: `epic`, `psn` (Playstation), `xbl` (Xbox), `steam`, `nsw` (Nintendo Switch) <br/>
`prefix`: (required), the name you are searching for

---

_Example Response (shortened)_

```json
[
  {
    "accountId": "4735ce9132924caf8a5b17789b40f79c",
    "matches": [
      {
        "value": "Ninja",
        "platform": "epic"
      }
    ],
    "matchType": "exact",
    "epicMutuals": 0,
    "sortPosition": 0
  },
  {
    "accountId": "44b8b1acc3b24ea99563f40bf595051b",
    "matches": [
      {
        "value": "ninja",
        "platform": "steam"
      }
    ],
    "matchType": "exact",
    "epicMutuals": 0,
    "sortPosition": 2
  },
  {
    "accountId": "ea356ee28c0644daae90e52cd90f802b",
    "matches": [
      {
        "value": "Ninja29425",
        "platform": "epic"
      }
    ],
    "matchType": "prefix",
    "epicMutuals": 0,
    "sortPosition": 99
  }
]
```
