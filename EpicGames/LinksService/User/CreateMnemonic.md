## Links Service - Create User Mnemonic

URL: https://links-public-service-live.ol.epicgames.com/links/api/:namespace/author/:accountId \
Method: POST \
Auth Required: Yes (`links:{namespace}:{accountId} CREATE`)

```json
{
    "creatorName": "", // name of mnemonic creator "can be anything"
    "linkType": "", // the mnemonic type ex. "Creative:Island"
    "discoveryIntent": "", // optional can be "PUBLIC" or "PRIVATE" default "PUBLIC"
    "discriptionTags": [ "" ], // optional defaults to []
    "metadata": {} // the actual link metadata
}
```

## Path Parameter

`namespace`: For Fortnite it's 'fn' <br/>
`accountId`: Your Account Id

## Parameter

...

