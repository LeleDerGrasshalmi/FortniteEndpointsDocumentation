## ホットコンフィグ

ゲーム サービス MCP ホストを更新します。

URL: https://fn-hotconfigs.ogs.live.on.epicgames.com/hotconfigs/v2/:filename \
メソッド: GET \
認証の有無: No

## Path Parameters

`filename`:

| 環境        | ファイル名    | 説明                                   |
| ----------- | ------------ | ------------------------------------- |
| ci          | ci.json      |                                       |
| gamedev     | gamedev.json |                                       |
| livefn      | livefn.json  | This is what the Shipping Client uses |
| prod        | prod.json    |                                       |
| stage       | stage.json   |                                       |

---

__レスポンスの例__

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
