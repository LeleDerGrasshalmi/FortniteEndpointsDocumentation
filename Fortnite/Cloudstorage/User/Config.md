## Fortnite - Cloudstorage: User Config

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/cloudstorage/user/config \
Method: GET \
Auth Required: Yes (`fortnite:cloudstorage:user:config READ`)

---

_Example Response_

```json
{
  "lastUpdated": "2023-05-18T23:00:17.902Z",
  "disableV2": true,
  "isAuthenticated": true,
  "enumerateFilesPath": "/api/cloudstorage/user",
  "enableMigration": false,
  "enableWrites": true,
  "epicAppName": "Live",
  "transports": {
    "McpProxyTransport": {
      "name": "McpProxyTransport",
      "type": "ProxyStreamingFile",
      "appName": "fortnite",
      "isEnabled": true,
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
      "isEnabled": false,
      "isRequired": false,
      "isPrimary": false,
      "timeoutSeconds": 30,
      "priority": 30
    }
  }
}
```
