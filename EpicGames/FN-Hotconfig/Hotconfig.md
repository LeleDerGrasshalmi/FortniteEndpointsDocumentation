## FN Hotconfig

Updates the Game Service MCPs Host.

URL: https://fn-hotconfigs.ogs.live.on.epicgames.com/hotconfigs/v2/:filename \
Method: GET \
Auth Required: No

## Path Parameters

`filename`:

| Environment | Filename     | Description                           |
| ----------- | ------------ | ------------------------------------- |
| ci          | ci.json      |                                       |
| gamedev     | gamedev.json |                                       |
| livefn      | livefn.json  | This is what the Shipping Client uses |
| prod        | prod.json    |                                       |
| stage       | stage.json   |                                       |

---

_Example Response (`livefn.json`)_

```json
{
  "HotConfigData": [
    {
      "AppId": "livefn",
      "EpicApp": "FortniteLivefn",
      "Modules": [
        {
          "ModuleName": "GameServiceMcp",
          "Endpoints": {
            "Android": "fngw-mcp-gc-livefn.ol.epicgames.com",
            "DedicatedServer": "fngw-mcp-ds-livefn.ol.epicgames.com",
            "Default": "fngw-mcp-gc-livefn.ol.epicgames.com",
            "IOS": "fngw-mcp-gc-livefn.ol.epicgames.com",
            "Linux": "fngw-mcp-gc-livefn.ol.epicgames.com",
            "Mac": "fngw-mcp-gc-livefn.ol.epicgames.com",
            "PS4": "fngw-mcp-gc-livefn.ol.epicgames.com",
            "PS5": "fngw-mcp-gc-livefn.ol.epicgames.com",
            "Switch": "fngw-mcp-gc-livefn.ol.epicgames.com",
            "Windows": "fngw-mcp-gc-livefn.ol.epicgames.com",
            "XB1": "fngw-mcp-gc-livefn.ol.epicgames.com",
            "XSX": "fngw-mcp-gc-livefn.ol.epicgames.com",
            "XboxOneGDK": "fngw-mcp-gc-livefn.ol.epicgames.com"
          }
        }
      ]
    }
  ]
}
```
