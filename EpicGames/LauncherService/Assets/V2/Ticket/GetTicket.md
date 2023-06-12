## Launcher Service - Assets (V2): Get Ticket

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/v2/by-ticket/app/:appName \
Method: POST \
Auth Required: Yes (`launcher:download:app:{appName} READ`)

```json
{
  "signedTicket": "eyJzaGFyZElkIjoiZWdzIiwiYXJ0aWZhY3RJZCI6IkZvcnRuaXRlIiwiZ3JhbnRBY2Nlc3NUb0RlcGVuZGVuY2llcyI6ZmFsc2UsImV4cGlyZXNBdCI6IjIwMjMtMDYtMTFUMjA6MDk6MzJaIiwiYWNjb3VudElkIjoiOTRiMTU2OTUwNmIwNGY5Zjg1NTdhZjYxMWU4YzVlNDciLCJiaW5hcnlWZXJzaW9uIjoiKytGb3J0bml0ZStSZWxlYXNlLTI1LjAwLUNMLTI1OTA5NjIyLVdpbmRvd3MifQ==.NWQ5NGMxZGUwYzA0YTdkNTM0NTJjNzI4NzgwOWZkNzZkNDMwNDQ2NzE0NDk5NzkwNTBhZTBjYTk2MmM2NGRhZA==",
  "binaryVersion": "++Fortnite+Release-25.00-CL-25909622-Windows"
}
```

## Path Parameters

`appName`: The App Name (from Catalog Item), e.g. `Fortnite` for Fortnite

## Parameters

`signedTicket`: From [Creation](./CreateTicket.md) <br/>
`binaryVersion`: From [Creation](./CreateTicket.md) <br/>

> The `binaryVersion` (claim is `binaryVersion`) and the `appName` (claim is `artifactId`) can be extracted from the JWT

---

_Example Response_

```json
{
  "elements": [
    {
      "appName": "Fortnite",
      "buildVersion": "++Fortnite+Release-25.00-CL-25909622-Windows",
      "hash": "78cf23202befa88d526de0c8513fe12593f698a9",
      "useSignedUrl": false,
      "metadata": {
        "installationPoolId": "FortniteInstallationPool"
      },
      "manifests": [
        {
          "uri": "https://download2.epicgames.com/Builds/Fortnite/CloudDir/aR-p-XE-qiz2uidz3k636UNRwJ-eyg.manifest",
          "queryParams": [
            {
              "name": "Policy",
              "value": "eyJTdGF0ZW1lbnQiOiBbeyJSZXNvdXJjZSI6IiovQnVpbGRzL0ZvcnRuaXRlL0Nsb3VkRGlyL2FSLXAtWEUtcWl6MnVpZHozazYzNlVOUndKLWV5Zy5tYW5pZmVzdCIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTY4NjUxNDMwNH0sIklwQWRkcmVzcyI6eyJBV1M6U291cmNlSXAiOiIwLjAuMC4wLzAifX19XX0_"
            },
            {
              "name": "Signature",
              "value": "uxTIySXGe5977FS-VQ12uQ4PbuQh5z-bvts6r9Zt2SewPpFCcxBTGjfzJdSXwKNlu32ktnpAYZ5TljAQTp~W9AVxNnx9TWgA0eXdNrIXk~wBZFarkoA2liBTCjKutFBDHH-AJ~pmfC3vNCWI5Qiq90J7TZD-FqEwQr7wCQtgTgF3XrZhgw1tNfa9H7yPjV4GD5QyVBDsDX1WDJb3Q3vDVTQwfGKdDf6wCHRtPPCH0RSOtKaKcY1YQ6iclYtXDcI9JxGPQ04UWqqvUtQP3vhSvrNVqGjWcw-6rCYSE~TgJYqRCaJLhPNGP~LF~k7UH-fcXElHLFymz5Oq2ALgdT5Eag__"
            },
            {
              "name": "Key-Pair-Id",
              "value": "APKAJP7WU44FM4EHJYFQ"
            }
          ]
        }
      ]
    }
  ]
}
```
