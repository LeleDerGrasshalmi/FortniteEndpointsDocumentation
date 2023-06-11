## Launcher Service - Assets: Asset for Catalog Item

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/:platform/:catalogItemId/:appName \
Method: GET \
Auth Required: Yes (`launcher:download:{label}:{appName} READ`)

## Path Parameters

`platform`: See [Platforms](../README.md#data) <br/>
`catalogItemId`: The Catalog-Item Id, e.g. `4fe75bbc5a674f4f9b356b5c90567da5` for Fortnite <br/>
`appName`: The App Name (from Catalog Item), e.g. `Fortnite` for Fortnite

## Query Parameters

`label`: optional, The label, usually `Live`, defaults to `Production`

---

_Example Response (shortened)_

```json
{
  "appName": "Fortnite",
  "labelName": "Live-Windows",
  "buildVersion": "++Fortnite+Release-24.40-CL-25595478-Windows",
  "catalogItemId": "4fe75bbc5a674f4f9b356b5c90567da5",
  "metadata": {
    "installationPoolId": "FortniteInstallationPool"
  },
  "expires": "2023-06-01T20:05:31.563Z",
  "items": {
    "MANIFEST": {
      "signature": "Policy=eyJTdGF0ZW1lbnQiOiBbeyJSZXNvdXJjZSI6IiovQnVpbGRzL0ZvcnRuaXRlL0Nsb3VkRGlyL2ZWeEg0VE5Rbng4Q2Z6cTJHa0txMVZUSzFCUWVKdy5tYW5pZmVzdCIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTY4NTY0OTkzMX0sIklwQWRkcmVzcyI6eyJBV1M6U291cmNlSXAiOiIwLjAuMC4wLzAifX19XX0_&Signature=npRquoHVVZzo-dgomu-zVKeZM8o8j6yxrMG3o~nLuSlOC6lZNKx2SSsFHE4wkdGprDTU0o14vBWugeoLNpj-Uo8JxR9wWr7T~eg1j-30AKZNb5N5AHTnaYfeDeNDmzY1k2vax5Awhe2OJ7GDp9dRyEPnq6mP8gs82Ds5nmF070X9oBAjFFmn5h5lhSctD11McrHbiWCAD9lRnO5eW7qBjlqZSlQWAClt0pNSZuYElcxKW0T8yUyt7P8Ne1smPeDn4TvuFPUy1NE3zY9GMncrglnB1IGozokJpDPdKv-e5vRQD94awv7fA230Gq5XRCKSt9ZZNs-2qTFU84eNYoSRKg__&Key-Pair-Id=APKAJP7WU44FM4EHJYFQ",
      "distribution": "https://download.epicgames.com/",
      "path": "Builds/Fortnite/CloudDir/fVxH4TNQnx8Cfzq2GkKq1VTK1BQeJw.manifest",
      "hash": "10ae1d79304733f3fc0a7b406495502ccc52839c",
      "additionalDistributions": [
        "https://download2.epicgames.com/",
        "https://download3.epicgames.com/",
        "https://download4.epicgames.com/"
      ]
    },
    "CHUNKS": {
      "signature": "Policy=eyJTdGF0ZW1lbnQiOiBbeyJSZXNvdXJjZSI6IiovQnVpbGRzL0ZvcnRuaXRlL0Nsb3VkRGlyL2ZWeEg0VE5Rbng4Q2Z6cTJHa0txMVZUSzFCUWVKdy5tYW5pZmVzdCIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTY4NTY0OTkzMX0sIklwQWRkcmVzcyI6eyJBV1M6U291cmNlSXAiOiIwLjAuMC4wLzAifX19XX0_&Signature=npRquoHVVZzo-dgomu-zVKeZM8o8j6yxrMG3o~nLuSlOC6lZNKx2SSsFHE4wkdGprDTU0o14vBWugeoLNpj-Uo8JxR9wWr7T~eg1j-30AKZNb5N5AHTnaYfeDeNDmzY1k2vax5Awhe2OJ7GDp9dRyEPnq6mP8gs82Ds5nmF070X9oBAjFFmn5h5lhSctD11McrHbiWCAD9lRnO5eW7qBjlqZSlQWAClt0pNSZuYElcxKW0T8yUyt7P8Ne1smPeDn4TvuFPUy1NE3zY9GMncrglnB1IGozokJpDPdKv-e5vRQD94awv7fA230Gq5XRCKSt9ZZNs-2qTFU84eNYoSRKg__&Key-Pair-Id=APKAJP7WU44FM4EHJYFQ",
      "distribution": "https://download.epicgames.com/",
      "path": "Builds/Fortnite/CloudDir/fVxH4TNQnx8Cfzq2GkKq1VTK1BQeJw.manifest",
      "additionalDistributions": [
        "https://download2.epicgames.com/",
        "https://download3.epicgames.com/",
        "https://download4.epicgames.com/"
      ]
    }
  },
  "assetId": "Fortnite"
}
```
