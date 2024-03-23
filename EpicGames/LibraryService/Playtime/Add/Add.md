## Library Service - Add Artifact Playtime

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/playtime/account/:accountId \
Method: PUT \
Auth Required: Yes (`library:public:{accountId}:playtime UPDATE`)

```json
{
  "machineId": "5058da6a-4ee8-4370-967f-4bff47a77114",
  "artifactId": "Fortnite",
  "startTime": "2023-08-25T16:51:36.056Z",
  "endTime": "2023-08-25T18:13:56.495Z",
  "startSegment": true,
  "endSegment": true
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`machineId`: This is a UUIDv4 <br/>
`artifactId`: The Artifact Id, e.g. `Fortnite` for Fortnite (See [How to obtain it](../../README.md#obtaining-the-artifact-id)) <br/>
`startTime`: ISO Start Date (should not be that much before the end date, otherwhise it won't add the playtime) <br/>
`endTime`: ISO Date, likely the current Date <br/>
`startSegment`: Unknown, but EGL sets it to true <br/>
`endSegment`: Unknown, but EGL sets it to true

---

_Example Response_: Status 204
