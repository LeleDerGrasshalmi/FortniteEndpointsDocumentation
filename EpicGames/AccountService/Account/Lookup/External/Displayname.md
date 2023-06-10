## Account Service - Lookup by External Display Name

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/lookup/externalAuth/:externalAuthType/displayName/:displayName \
Method: GET \
Auth Required: Yes (`account:public:account:lookup:externalDisplayName:{externalAuthType} READ`)

## Query Parameters

`caseInsensitive`: boolean (optional), just make it always true, theres no reason to care about the exact case

## Path Parameters

`externalAuthType`: See via [External Auth Readme](../../ExternalAuth/README.md) <br/>
`displayName`: External Provider User Displayname

---

_Example Response_

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
