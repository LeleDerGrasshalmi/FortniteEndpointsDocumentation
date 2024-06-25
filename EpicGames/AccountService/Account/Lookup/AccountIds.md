## Account Service - Lookup by Account Ids

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account \
Method: GET \
Auth Required: Yes (No Permission required)

## Query Parameters

`accountId`: Account Ids, you can use the query multiple times **[Max 100 per Request]**

---

_Example Response_

```json
[
  {
    "id": "020b5d9042174a7692f20db8e23b84d1",
    "displayName": "nintendo test ac",
    "externalAuths": {
      "nintendo": {
        "accountId": "020b5d9042174a7692f20db8e23b84d1",
        "type": "nintendo",
        "externalAuthIdType": "nintendo_id",
        "authIds": []
      }
    }
  },
  {
    "id": "881f4d75aa3046c5b648a73aea641e69",
    "displayName": "GXR Malibuca",
    "externalAuths": {
      "steam": {
        "accountId": "881f4d75aa3046c5b648a73aea641e69",
        "type": "steam",
        "externalAuthId": "76561198253493804",
        "externalAuthIdType": "steam_id64",
        "externalAuthSecondaryId": "6DE753B959A9386A14EB3D2A8B3B665AFC5655B2",
        "externalDisplayName": "Malibuca (rus)",
        "avatar": "c58668dcea116885804b27c9e3abdc4c09cc7ee4",
        "authIds": [
          {
            "id": "76561198253493804",
            "type": "steam_id64"
          },
          {
            "id": "6DE753B959A9386A14EB3D2A8B3B665AFC5655B2",
            "type": "steam_id64_hash"
          }
        ]
      },
      "psn": {
        "accountId": "881f4d75aa3046c5b648a73aea641e69",
        "type": "psn",
        "externalAuthId": "3023845316854687677",
        "externalAuthIdType": "psn_user_id",
        "externalDisplayName": "GXRmalibucafn",
        "authIds": [
          {
            "id": "3023845316854687677",
            "type": "psn_user_id"
          }
        ]
      }
    }
  }
]
```
