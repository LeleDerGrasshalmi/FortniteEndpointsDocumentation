## Links Service - Create User Mnemonic

URL: https://links-public-service-live.ol.epicgames.com/links/api/:namespace/author/:accountId \
Method: POST \
Auth Required: Yes (`links:{namespace}:{accountId} CREATE`)

```json
{
  "creatorName": "Lele",
  "linkType": "Creative:Island",
  "metadata": {},
  "descriptionTags": ["pve"],
  "discoveryIntent": "PRIVATE"
}
```

## Path Parameters

`namespace`: For Fortnite it's 'fn' <br/>
`accountId`: Your Account Id

## Parameters

`creatorName`: required - Creators name <br/>
`linkType`: required - the type of the Link e.g. 'valkyrie:application' (UEFN Project) or 'Creative:Island' (Creative V1 Island) <br/>
`metadata`: required - Main Link Metadata (Type is `Record<string, object>`) <br/>
`descriptionTags`: optional - Array of Tags (Strings), the example above shows the tags for StW <br/>
`discoveryIntent`: optional - valid Values: `PUBLIC` (Default) or `PRIVATE`

---

_Example Response (shortened)_

```json
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
```
