## Lightswitch Service - Status (Bulk)

URL: https://lightswitch-public-service-prod06.ol.epicgames.com/lightswitch/api/service/bulk/status \
Method: GET \
Auth Required: Yes (no perm needed)

## Query Parameters

`serviceId`: You can use the query multiple times. See [Readme](../README.md) for examples

---

_Example Response_

```json
[
  {
    "serviceInstanceId": "kairos",
    "status": "DOWN",
    "message": "Farewell. Thank you for all the memories.",
    "maintenanceUri": null,
    "overrideCatalogIds": ["a7f138b2e51945ffbfdacc1af0541053"],
    "allowedActions": [],
    "banned": false,
    "launcherInfoDTO": null
  },
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
]
```
