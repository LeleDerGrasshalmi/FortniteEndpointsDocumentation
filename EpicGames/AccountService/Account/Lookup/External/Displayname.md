## アカウントサービス-外部表示名の検索

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/lookup/externalAuth/:externalAuthType/displayName/:displayName \
メソッド: GET \
認証の有無: Yes (`account:public:account:lookup:externalDisplayName:{externalAuthType} READ`)

## クエリパラメータ

`caseInsensitive`: boolean。つねにtrueにするだけで、特に気にかける必要はありません。

## パスパラメータ

`externalAuthType`:  [こちら](../../ExternalAuth/README.md) を参照してください。<br/>
`displayName`: 外部プロバイダーのディスプレイネーム

---

__レスポンス例__

```json
[
  {
    "id": "bec13864ce1d44148e04cb82401c4257",
    "displayName": "code jem",
    "links": {},
    "externalAuths": {
      "xbl": {
        "accountId": "bec13864ce1d44148e04cb82401c4257",
        "type": "xbl",
        "externalAuthIdType": "xuid",
        "externalDisplayName": "jemcer",
        "authIds": []
      },
      "nintendo": {
        "accountId": "bec13864ce1d44148e04cb82401c4257",
        "type": "nintendo",
        "externalAuthId": "lp1_e61ac60c1a63b71e",
        "externalAuthIdType": "nsa_id",
        "authIds": [
          {
            "id": "lp1_e61ac60c1a63b71e",
            "type": "nsa_id"
          }
        ]
      },
      "psn": {
        "accountId": "bec13864ce1d44148e04cb82401c4257",
        "type": "psn",
        "externalAuthId": "3940490760434152335",
        "externalAuthIdType": "psn_user_id",
        "externalDisplayName": "jemcer_ps",
        "authIds": [
          {
            "id": "3940490760434152335",
            "type": "psn_user_id"
          }
        ]
      }
    }
  }
]
```
