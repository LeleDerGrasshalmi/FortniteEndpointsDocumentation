# Get Affiliate Profile

URL: https://sac.epicgames.com/api/get-profile \
Method: GET \
Auth Required: Yes

---

_Example Response_

```json
{
  "data": {
    "id": "0d2ccb730f2f4fac82d04bb7bb8d2d80",
    "slug": "this is lele",
    "status": "ACTIVE",
    "personalInfo": {
      "minor": true,
      "guardian": {
        "firstName": "M***h",
        "lastName": "M***h",
        "relationship": "father"
      }
    },
    "payeeSetupInfo": {
      "completed": true,
      "firstSetupCompleted": true,
      "dueDate": null,
      "taxProfileStatus": "COMPLETED",
      "taxProfileStatusOriginalValue": "TAX_VERIFIED",
      "walletStatus": "COMPLETED",
      "walletStatusOriginalValue": "ACCOUNT_ACTIVATED",
      "paymentConsent": true
    },
    "earningsInfo": {
      "earningsWindowStart": "2022-10-01T00:00:00.000Z",
      "earningsDeadline": "2023-09-30T23:59:59.999Z"
    },
    "programs": {
      "media": {
        "id": "0d2ccb730f2f4fac82d04bb7bb8d2d80",
        "disabledReason": null,
        "earliestReapplicationAt": null,
        "lifecycle": {
          "signupCompleted": true,
          "firstPayeeSetupCompleted": true,
          "canEditSettings": true,
          "newAgreements": []
        },
        "oauthInfo": {
          "violatedAt": null,
          "lastCheckDate": "2023-09-14T16:30:24.979Z",
          "fixDueDate": null,
          "fixRemindedAt": null
        },
        "socialChannels": [
          {
            "id": "dd29ebbdd1354c268736697e653b7a6f",
            "platform": "YOUTUBE_CHANNEL",
            "url": "https://www.youtube.com/channel/UClG8odDC8TS6Zpqk9CGVQiQ",
            "followers": 11500000,
            "mainChannel": true,
            "oauthDetails": {
              "valid": true
            },
            "status": "VALID",
            "createdAt": "2023-09-14T15:24:42.582Z"
          }
        ],
        "createdAt": "2022-09-14T16:24:40.554Z",
        "agreementDecisions": [
          {
            "agreementType": "SAC",
            "agreementReleaseOrder": 2,
            "date": "2022-09-14T16:24:40.554Z",
            "decision": "ACCEPT",
            "voluntary": true,
            "eulaSvcKey": "sac_agreement",
            "eulaSvcVersion": 1,
            "agreementFriendlyType": "SAC",
            "agreementFriendlyVersion": "2.0",
            "agreementFriendlyName": "SAC 2.0"
          }
        ]
      }
    },
    "createdAt": "2022-09-14T16:24:40.554Z",
    "portedEcpCreator": true,
    "oauthInfo": {
      "violatedAt": null,
      "lastCheckDate": "2030-01-01T00:00:00.000Z",
      "fixDueDate": null,
      "fixRemindedAt": null
    }
  },
  "success": true
}
```
