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
      "buildVersion": "++Fortnite+Release-41.00-CL-54618515-Windows",
      "hash": "b129378b03c7a85f5633b41ad5467d851ba8e86c",
      "useSignedUrl": false,
      "metadata": {
        "installationPoolId": "FortniteInstallationPool",
        "hasDependencyConfig": true
      },
      "manifests": [
        {
          "uri": "https://egs-cloudfront-chunks.epicgamescdn.com/Builds/Fortnite/CloudDir/UcaaeP2Bi8ObrwuT60SrYiVf3NGxXA.manifest",
          "queryParams": [
            {
              "name": "cf_token",
              "value": "1780723395_70f97c1833b3e36042a9282e61a8b0a4d65e895c"
            }
          ]
        }
      ],
      "selectiveDownload": [
        {
          "uri": "https://selective-download-egs.distro.on.epicgames.com/Org/o-aa83a0a9bc45e98c80c1b1c9d92e9e/Product/prod-fn/da/da1703a0b71dec81b397e187559a5f0dfc2774f19f7f665cee8512657511ccd8.sdmeta",
          "queryParams": [
            {
              "name": "cf_token",
              "value": "1780723395_612a0aa15358699157c96e2f9ffc5e7ed0246157"
            }
          ]
        }
      ],
      "isPreloaded": false
    }
  ]
}
```
