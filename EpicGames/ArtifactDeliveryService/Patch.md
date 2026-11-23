## Artifact Delivery Service - Patch

URL: https://artifact-delivery-public-service-prod.beee.live.use1a.on.epicgames.com/artifact-delivery/api/public/v1/delivery/account/:accountId/patch <br/>
Method: POST <br/>
Auth Required: Yes (`delivery:public:patch:{accountId} READ`)

```json
{
  "signedTicket": "eyJzaGFyZElkIjoiZWdzIiwiYXJ0aWZhY3RJZCI6IkZvcnRuaXRlIiwiZ3JhbnRBY2Nlc3NUb0RlcGVuZGVuY2llcyI6ZmFsc2UsImV4cGlyZXNBdCI6IjIwMjUtMTAtMDhUMDk6MzU6MjNaIiwiYWNjb3VudElkIjoiNWYzOGMzMTI3YzhmNDRmOWI1OWFlMzNiMDk1ZDYwYjAiLCJiaW5hcnlWZXJzaW9uIjoiKytGb3J0bml0ZStSZWxlYXNlLTM3LjQwLUNMLTQ2Mjk1NjczLVdpbmRvd3MifQ==.ZWVjZDlhNjZjMzU1ODI1Y2U0YTVkYjczMzRiY2VjZTAyZDE5ZGM0MDJjZDhhNGM4NTcyNjZjMGRlZTUzOWY1ZQ==",
  "deltaId": "F2HLp1AT9ECKev6viRB5_A/OBkNfoIsGkeguepJAsUBlw.delta"
}
```

## Path Parameters

`accountId`: Your account ID.

## Parameters

`signedTicket`: The signed ticket returned by the [Launcher Service Ticket API](../LauncherService/Assets/V2/Ticket/CreateTicket.md). <br/>
`deltaId`: The delta ID in `targetBuildId/baseBuildId.delta` format.

---

*Example Response (shortened)*

```json
{
  "artifactId": "Fortnite",
  "binaryVersion": "++Fortnite+Release-37.40-CL-46295673-Windows",
  "distributionPoints": [
    {
      "patchUrl": "https://fastly-download.epicgames.com/Builds/Fortnite/CloudDir/Deltas/F2HLp1AT9ECKev6viRB5_A/OBkNfoIsGkeguepJAsUBlw.delta?f_token=REDACTED",
      "signatureExpiration": "2025-10-08T09:35:59.889Z"
    }
  ]
}
```
