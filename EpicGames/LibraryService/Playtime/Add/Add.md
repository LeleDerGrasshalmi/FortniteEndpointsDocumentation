## Library Service - Add Artifact Playtime

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/playtime/account/:accountId \
Method: PUT \
Auth Required: Yes (`library:public:{accountId}:playtime UPDATE`)

```json
{
  "machineId": "0327b13a-27c1-41a0-9478-5c7cf125c48c",
  "startTime": "2023-08-25T16:51:36.056Z",
  "endTime": "2023-08-25T18:10:16.254Z",
  "artifactId": "Fortnite"
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`machineId`: UUIDv4? <br/>
`startTime`: ISO Start Date (should not be that much before the end date, otherwhise it won't add the playtime) <br/>
`endTime`: ISO Date, likely the current Date <br/>
`artifactId`: The Artifact Id, e.g. `Fortnite` for Fortnite (See [How to obtain it](../../README.md#obtaining-the-artifact-id))

---

_Example Response_: Status 204
