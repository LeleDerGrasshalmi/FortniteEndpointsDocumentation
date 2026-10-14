## EOS SDK Config Service - Default Config

URL: https://api.epicgames.dev/sdk/v1/default \
Method: GET \
Auth Required: No

---

_Example Response (shortened)_

```json
{
  "client": {
    "BaseService": {
      "HttpRetryLimit": 4,
      "HttpRetryResponseCodes": [
        429,
        503,
        504
      ]
    },
    "Messaging.EpicConnect": {
      "Url": "wss://connect.epicgames.dev",
      "Urlv2": "wss://connect.epicgames.dev/v2",
      "UseV2Connection": false,
      "ClientHeartbeatIntervalMilliseconds": 30000
    }
  },
  "services": {
    "AccountsEpicIdService": {
      "BaseUrl": "https://api.epicgames.dev"
    },
    "PartiesService": {
      "BaseUrl": "https://api.epicgames.dev/epic/party"
    },
    "PartiesInternalService": {
      "BaseUrl": "https://api.epicgames.dev/epic/party/internal"
    },
    "PresenceService": {
      "BaseUrl": "https://api.epicgames.dev/epic/presence"
    },
    "RTCService": {
      "BaseUrl": "https://api.epicgames.dev/rtc"
    },
    "TextChatTrustedServerFNService": {
      "BaseUrl": "https://api.epicgames.dev/epic/chat"
    }
  },
  "watermark": 794601937
}
```
