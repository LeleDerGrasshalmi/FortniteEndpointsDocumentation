## Launcher Service - Assets (V2): Get Item Build Simple

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/v2/platform/:platform/catalogItem/:catalogItemId/app/:appName \
Method: GET \
Auth Required: Yes (`launcher:download:{label}:{appName} READ`)

## Path Parameters

`platform`: See [Platforms](../../README.md#data) <br/>
`namespace`: The Catalog Namespace, e.g. `fn` for Fortnite <br/>
`catalogItemId`: The Catalog-Item Id, e.g. `4fe75bbc5a674f4f9b356b5c90567da5` for Fortnite <br/>
`appName`: The App Name (from Catalog Item), e.g. `Fortnite` for Fortnite

## Query Parameters

`label`: optional, The label, usually `Live`, defaults to `Production`

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
          "uri": "https://epicgames-download1.akamaized.net/Builds/Fortnite/CloudDir/aR-p-XE-qiz2uidz3k636UNRwJ-eyg.manifest",
          "queryParams": [
            {
              "name": "ak_token",
              "value": "exp=1686513741~hmac=41d877f36622f4527fb9b3b7a8baaa6fef95ee7cb68650964c2b5db7cd9aab15"
            }
          ]
        }
      ]
    }
  ]
}
```
