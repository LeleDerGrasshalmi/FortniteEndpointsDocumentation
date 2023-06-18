## Links Service - User Mnemonics

URL: https://links-public-service-live.ol.epicgames.com/links/api/:namespace/author/:accountId \
Method: GET \
Auth Required: Yes (`links:{namespace}:{accountId} READ`)

## Path Parameters

`namespace`: For Fortnite it's 'fn' <br/>
`accountId`: Your Account Id

---

_Example Response (shortened)_

```json
[
  {
    "namespace": "fn",
    "accountId": "",
    "creatorName": "",
    "mnemonic": "4247-4800-9493",
    "linkType": "valkyrie:application",
    "metadata": {},
    "version": 1,
    "active": true,
    "disabled": false,
    "created": "2023-03-29T20:11:00.102Z",
    "published": "2023-03-29T20:11:00.102Z",
    "descriptionTags": [],
    "moderationStatus": "Unmoderated",
    "lastActivatedDate": "2023-03-29T20:11:00.105Z",
    "discoveryIntent": "PUBLIC"
  }
]
```
