## Library Service - Add Playtime (Bulk)

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/playtime/account/:accountId/bulk \
Method: PUT \
Auth Required: Yes (`library:public:{accountId}:playtime UPDATE`)

```json
{
  "playtimeAddList": [
    {
      "machineId": "5058da6a-4ee8-4370-967f-4bff47a77114",
      "artifactId": "Fortnite",
      "startTime": "2023-08-25T16:51:36.056Z",
      "endTime": "2023-08-25T18:13:56.495Z",
      "startSegment": true,
      "endSegment": true
    }
  ]
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`playtimeAddList[].machineId`: This is a UUIDv4 <br/>
`playtimeAddList[].artifactId`: The Artifact Id, e.g. `Fortnite` for Fortnite (See [How to obtain it](../../README.md#obtaining-the-artifact-id)) <br/>
`playtimeAddList[].startTime`: ISO Start Date (should not be that much before the end date, otherwhise it won't add the playtime) <br/>
`playtimeAddList[].endTime`: ISO Date, likely the current Date <br/>
`playtimeAddList[].startSegment`: Unknown, but EGL sets it to true <br/>
`playtimeAddList[].endSegment`: Unknown, but EGL sets it to true

---

_Example Response_: Status 204

The interval is added to the artifact's total right away (a 2 minute interval raised `totalTime` from [Artifact Playtime](../Info/Artifact.md) by exactly 120). An interval whose `endTime` is before its `startTime` also returns 204 but adds nothing.

_Example Response (`playtimeAddList` empty)_

```json
{
  "errorCode": "errors.com.epicgames.library.missing_argument",
  "errorMessage": "playtimeAddList must be supplied with the request.",
  "messageVars": [],
  "numericErrorCode": 53001,
  "originatingService": "library-service",
  "intent": "prod"
}
```

A missing `machineId` returns the same error with `machineId must be supplied with the request.`
