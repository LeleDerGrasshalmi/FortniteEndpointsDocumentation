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
            "Android": "mcp-gc.live.fngw.ol.epicgames.com",
            "DedicatedServer": "mcp-ds.live.fngw.ol.epicgames.com",
            "Default": "mcp-gc.live.fngw.ol.epicgames.com",
            "IOS": "mcp-gc.live.fngw.ol.epicgames.com",
            "Linux": "mcp-gc.live.fngw.ol.epicgames.com",
            "Mac": "mcp-gc.live.fngw.ol.epicgames.com",
            "PS4": "mcp-gc.live.fngw.ol.epicgames.com",
            "PS5": "mcp-gc.live.fngw.ol.epicgames.com",
            "Switch": "mcp-gc.live.fngw.ol.epicgames.com",
            "Windows": "mcp-gc.live.fngw.ol.epicgames.com",
            "XB1": "mcp-gc.live.fngw.ol.epicgames.com",
            "XSX": "mcp-gc.live.fngw.ol.epicgames.com",
            "XboxOneGDK": "mcp-gc.live.fngw.ol.epicgames.com"
          }
        }
      ]
    }
  ]
}
```
