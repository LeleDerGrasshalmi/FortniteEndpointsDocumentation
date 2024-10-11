## FN Service - Cloudstorage: User Config

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/cloudstorage/user/config \
Method: GET \
Auth Required: Yes (`fortnite:cloudstorage:user:config READ`)

---

_Example Response_

```json
{
  "lastUpdated": "2024-10-11T19:38:41.720Z",
  "disableV2": false,
  "isAuthenticated": true,
  "enumerateFilesPath": "/api/cloudstorage/user",
  "enableMigration": true,
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
