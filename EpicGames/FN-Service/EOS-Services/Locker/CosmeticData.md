## FN EOS Locker Service: Cosmetic Data

URL: https://fngw-svc-gc-livefn.ol.epicgames.com/api/locker/v4/:deploymentId/account/:accountId/cosmetic-data \
Method: GET \
Auth Required: Yes (`locker:items`)

## Path Parameters

`deploymentId`: The Deployment Id from env configuration, for `live-fn` it is `62a9473a2dca46b29ccf17577fcf42d7` <br/>
`accountId`: Your Account Id

---

_Example Response (shortened)_

```json
{
    "cosmeticItems": [{
            "templateId": "AthenaBackpack:backpack_abstractmirror",
            "cosmeticItemId": "AthenaBackpack:backpack_abstractmirror",
            "athenaItemId": "15f3e2c8-d8a6-40e2-a557-b93c16f75a66",
            "updatedTime": "2025-06-13T06:42:43.662179648Z",
            "activeVariants": {}
        },
        {
            "templateId": "AthenaBackpack:backpack_agentsherbert",
            "cosmeticItemId": "AthenaBackpack:backpack_agentsherbert",
            "athenaItemId": "cceefb74-419d-4981-b643-00b7d519283c",
            "updatedTime": "2025-06-13T06:42:43.659017136Z",
            "ownedVariants": {
                "Progressive": [{
                        "variantTag": "Stage1"
                    },
                    {
                        "variantTag": "Stage2"
                    }
                ]
            },
            "activeVariants": {
                "Progressive": {
                    "variantTag": "Stage1"
                }
            }
        },
        {
            "templateId": "AthenaBackpack:backpack_pajamasoar",
            "cosmeticItemId": "AthenaBackpack:backpack_pajamasoar",
            "athenaItemId": "1bdbc2e0-5320-46e8-bde8-24412ef9b2be",
            "creationTime": "2025-08-26T15:43:16.446Z",
            "updatedTime": "2025-08-26T15:44:24.001372477Z",
            "activeVariants": {},
            "lockedIn": false
        }
    ],
    "cosmeticItemAccessTokens": [],
    "requestTime": "2026-03-25T18:02:33.918574015Z",
    "nextToken": "Ywko2REqD3h09F89MY-GwdS3ZdbEVcjvwNowbUKqFxFdVB-UR57s028k_ftoVOVIExTk4FbU_WQA9u3xB0lwuoItw_c7gaQkfNeFO6l_TF4NHjKUW9Kc4gLpAWdoudL6HMGQeAvVfUUMmew4l33Q5kC1CV72C9eDd_Q7lB42eGdCNTI9IqcADOPCMKwJEqpX1gQHrnaQOAOVtj8S5XLq6lVDtY-Mja8wqdqhKZf-oZzV6dMgxzrjFXllfOCGtjN2"
}
```
