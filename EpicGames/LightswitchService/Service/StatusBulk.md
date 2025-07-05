## フォートナイトサーバーステータス-一括取得

URL: https://lightswitch-public-service-prod06.ol.epicgames.com/lightswitch/api/service/bulk/status \
メソッド: GET \
認証の有無: Yes (no perm needed)

**APIカテゴリ:ライトスイッチ**

## クエリパラメータ

`serviceId`: [こちら](../README.md)を参照してください。また、クエリは複数の指定が可能です。

---

__レスポンスの例__

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
