## Links Service - Create User Mnemonic

URL: https://links-public-service-live.ol.epicgames.com/links/api/:namespace/author/:accountId \
Method: POST \
Auth Required: Yes (`links:{namespace}:{accountId} CREATE`)

```json
{
  "creatorName": "Lele",
  "linkType": "Creative:Island",
  "metadata": {},
  "descriptionTags": [],
  "discoveryIntent": "PRIVATE"
}
```

## Path Parameter

`namespace`: For Fortnite it's 'fn' <br/>
`accountId`: Your Account Id

## Parameter

`creatorName`: required - Creators name <br/>
`linkType`: required - the type of the Link e.g. 'valkyrie:application' (UEFN Project) or 'Creative:Island' (Creative V1 Island) <br/>
`metadata`: required - Main Link Metadata <br/>
`descriptionTags`: optional - Array of Tags (Strings) e.g. ["pve"] (StW) <br/>
`discoveryIntent`: optional - valid Values: "**PUBLIC**" (Default) or "**PRIVATE**"
