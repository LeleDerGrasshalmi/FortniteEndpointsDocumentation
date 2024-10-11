## FN Service - Cloudstorage: System Config

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/cloudstorage/system/config \
Method: GET \
Auth Required: Yes (`fortnite:cloudstorage:system READ`)

---

_Example Response_

```json
{
  "lastUpdated": "2024-10-11T19:34:56.833Z",
  "disableV2": false,
  "isAuthenticated": true,
  "enumerateFilesPath": "/api/cloudstorage/system",
  "enableMigration": false,
  "enableWrites": false,
  "epicAppName": "Live",
  "transports": {
    "McpProxyTransport": {
      "name": "McpProxyTransport",
      "type": "ProxyStreamingFile",
      "appName": "fortnite",
      "isEnabled": false,
      "isRequired": true,
      "isPrimary": true,
      "timeoutSeconds": 30,
      "priority": 10
    },
    "McpSignatoryTransport": {
      "name": "McpSignatoryTransport",
      "type": "ProxySignatory",
      "appName": "fortnite",
      "isEnabled": false,
      "isRequired": false,
      "isPrimary": false,
      "timeoutSeconds": 30,
      "priority": 20
    },
    "DssDirectTransport": {
      "name": "DssDirectTransport",
      "type": "DirectDss",
      "appName": "fortnite",
      "isEnabled": true,
      "isRequired": false,
      "isPrimary": false,
      "timeoutSeconds": 30,
      "priority": 30
    }
  }
}
```
