## Launcher Service - Assets (V2): Get Item Build

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/v2/platform/:platform/namespace/:namespace/catalogItem/:catalogItemId/app/:appName/label/:label \
Method: GET \
Auth Required: Yes (`launcher:download:{label}:{appName} READ`)

## Path Parameters

`platform`: See [Platforms](../../README.md#data) <br/>
`namespace`: The Catalog Namespace, e.g. `fn` for Fortnite <br/>
`catalogItemId`: The Catalog-Item Id, e.g. `4fe75bbc5a674f4f9b356b5c90567da5` for Fortnite <br/>
`appName`: The App Name (from Catalog Item), e.g. `Fortnite` for Fortnite <br/>
`label`: The label, usually `Live`, defaults to `Production`

---

_Example Response (shortened)_

```json
{
  "elements": [
    {
      "appName": "Fortnite",
      "labelName": "Live-Windows",
      "buildVersion": "++Fortnite+Release-25.00-CL-25909622-Windows",
      "hash": "78cf23202befa88d526de0c8513fe12593f698a9",
      "useSignedUrl": false,
      "metadata": {
        "installationPoolId": "FortniteInstallationPool"
      },
      "manifests": [
        {
          "uri": "https://fastly-download.epicgames.com/Builds/Fortnite/CloudDir/aR-p-XE-qiz2uidz3k636UNRwJ-eyg.manifest",
          "queryParams": [
            {
              "name": "f_token",
              "value": "1686504874_9bfccefe1826c0ee223e154c62c0a54e9dbccc13"
            }
          ]
        }
      ]
    }
  ]
}
```
