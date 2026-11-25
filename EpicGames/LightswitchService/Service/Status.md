## Lightswitch Service - Status

URL: https://lightswitch-public-service-prod.ol.epicgames.com/lightswitch/api/service/:serviceId/status <br/>
Method: GET <br/>
Auth Required: Yes (no perm needed)

## Path Parameters

`serviceId`: See [Readme](../README.md) for examples

---

*Example Response*

```json
{
  "serviceInstanceId": "fortnite",
  "status": "UP",
  "message": "Fortnite is online",
  "maintenanceUri": null,
  "overrideCatalogIds": ["a7f138b2e51945ffbfdacc1af0541053"],
  "allowedActions": [],
  "banned": false,
  "launcherInfoDTO": {
    "appName": "Fortnite",
    "catalogItemId": "4fe75bbc5a674f4f9b356b5c90567da5",
    "namespace": "fn"
  }
}
```
