## Account Service - Auth: Device Auth Info

URL: https://account-public-service-prod.ol.epicgames.com/account/api/public/account/:accountId/deviceAuth/:deviceId \
Method: GET \
Auth Required: Yes (`account:public:account:deviceAuths READ`)

---

_Example Response_

```json
{
  "deviceId": "06b96e4c93ce452590408e72f814dedf",
  "accountId": "94b1569506b04f9f8557af611e8c5e47",
  "userAgent": "Fortnite/++Fortnite+Release-24.40-CL-25549531 Windows/10.0.19042.1.768.64bit",
  "created": {
    "location": "Germany",
    "ipAddress": "127.0.0.1",
    "dateTime": "2023-05-23T15:18:27.346Z"
  },
  "lastAccess": {
    "location": "Germany",
    "ipAddress": "127.0.0.1",
    "dateTime": "2023-08-30T08:00:05.314Z"
  }
}
```
