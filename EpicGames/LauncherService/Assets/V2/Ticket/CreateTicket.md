## Launcher Service - Assets (V2): Create Ticket

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/v2/ticket \
Method: POST \
Auth Required: Yes (`launcher:download:label:{label}:app:{appName}:ticket CREATE`)

```json
{
  "appName": "Fortnite",
  "catalogItemId": "4fe75bbc5a674f4f9b356b5c90567da5",
  "namespace": "fn",
  "platform": "Windows",
  "label": "Live",
  "buildVersion": "++Fortnite+Release-25.00-CL-25909622-Windows"
}
```

## Parameters

`appName`: The App Name (from Catalog Item), e.g. `Fortnite` for Fortnite <br/>
`catalogItemId`: The Catalog-Item Id, e.g. `4fe75bbc5a674f4f9b356b5c90567da5` for Fortnite <br/>
`namespace`: The Catalog Namespace, e.g. `fn` for Fortnite <br/>
`platform`: See [Platforms](../../../README.md#data) <br/>
`label`: The label, usually `Live`, defaults to `Production` <br/>
`buildVersion`: The Latest Build-Version of the Catalog Item

---

_Example Response_

```json
{
  "signedTicket": "eyJzaGFyZElkIjoiZWdzIiwiYXJ0aWZhY3RJZCI6IkZvcnRuaXRlIiwiZ3JhbnRBY2Nlc3NUb0RlcGVuZGVuY2llcyI6ZmFsc2UsImV4cGlyZXNBdCI6IjIwMjMtMDYtMTFUMjA6MDU6NDdaIiwiYWNjb3VudElkIjoiOTRiMTU2OTUwNmIwNGY5Zjg1NTdhZjYxMWU4YzVlNDciLCJiaW5hcnlWZXJzaW9uIjoiKytGb3J0bml0ZStSZWxlYXNlLTI1LjAwLUNMLTI1OTA5NjIyLVdpbmRvd3MifQ==.Njg2YzZkZGRhZjg2OTc5NjU4ZDQxNjYxNzYwN2IzN2RiMzE5NTIzOTMzMGUzZTMwODM1NzY1YzRiY2Q2NDc5NQ==",
  "expiresAt": "2023-06-11T20:05:47Z"
}
```
