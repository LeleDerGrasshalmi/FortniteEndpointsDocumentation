## Party Service - Send Request To Join

URL: https://party-service-prod.ol.epicgames.com/party/api/v1/Fortnite/members/:friendId/intentions/:accountId \
Method: POST \
Auth Required: Yes (`social:party`)

```json
{
    "urn:epic:invite:platformdata_s": "",
}
```

## Path Parameters

`friendId`: Friend AccountId <br/>
`accountId`: Your AccountId

## Parameters

`urn:epic:invite:platformdata_s`: Always empty