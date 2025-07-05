## フォートナイトサーバーステータス

URL: http://lightswitch-public-service-prod.ol.epicgames.com/lightswitch/api/service/:serviceId/status \
メソッド: GET \
認証の有無: Yes (no perm needed)

**APIカテゴリ:ライトスイッチサービス**

## パスパラメータ

`serviceId`:  [こちら](../README.md) を参照してください。

---

__レスポンスの例(サーバーがオンラインの場合)__

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

__レスポンスの例(サーバーがオフラインの場合)__

```json
{
  "serviceInstanceId": "fortnite",
  "status": "down",
  "message": "Fortnite is offline",
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
