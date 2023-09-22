## Account Web - Authorized Apps

URL: https://www.epicgames.com/account/v2/authorized-apps \
Method: GET \
Auth Required: Yes

_Example Response_

```json
{
  "success": true,
  "data": {
    "applications": [
      {
        "createdAt": "2023-09-14T16:41:32.693422Z",
        "applicationName": "LEGO Account",
        "applicationId": "fghi4567GYGhtxRcfmxj24NZaEbaluZj",
        "privacyPolicy": "https://identity.lego.com/terms",
        "applicationWebsite": "https://identity.lego.com/",
        "logo": "https://media-cdn.epicgames.com/c254be4e7ef64548a128650d21aa666b/logo-927c5761667742079eb7050054a1c9b2-57536341839f482786f56220a42f8d4e.png",
        "isPlatform": true
      },
      {
        "createdAt": "2023-08-06T11:01:16.260054Z",
        "applicationName": "Metahuman Creator",
        "applicationId": "fghi4567EOGZaXhObgIBhUpmbygpOJcY",
        "privacyPolicy": "https://www.epicgames.com/site/en-US/privacypolicy",
        "logo": "https://media-cdn.epicgames.com/cbae237da245453c98848204a9c8ed52/logo-dcefb0c74843459babdefcd05b4c2f46-c7b1fc3313f74063b96a582c5b54b32e.png"
      },
      {
        "createdAt": "2023-08-04T02:48:45.449089Z",
        "applicationName": "Fortnite Discord Quest",
        "applicationId": "fghi45676lvzDF8dmFYQ18oAyU3KQaof",
        "privacyPolicy": "https://fdquests.com/privacypolicy",
        "applicationWebsite": "https://fdquests.com/",
        "logo": "https://media-cdn.epicgames.com/5f2b2f8fe6924365b3ad0dce06fb0abf/logo-48b97c53e35948ddbd6ea79b1f70a345-beb0a65dbb3340428ee9ea223c3a4951.png"
      },
      {
        "createdAt": "2023-01-24T11:31:17.537941Z",
        "applicationName": "Maestro",
        "applicationId": "fghi4567dxSakdbhAFQxcLDkvYgmpNXU",
        "supportEmail": "https://support.maestro.io",
        "privacyPolicy": "https://info.maestro.io/privacy"
      },
      {
        "createdAt": "2000-11-26T01:01:48.399382Z",
        "applicationName": "Discord",
        "applicationId": "fghi4567VehIJXAetZHjKxO0fk9ZZqj8",
        "privacyPolicy": "https://discord.com/privacy",
        "applicationWebsite": "https://discord.com/",
        "logo": "https://media-cdn.epicgames.com/e1a9edf92c39489fb09bfe68f7d7dda8/logo-4ead462496784fe082f3de3790862701-3c752349cd4242f5b238221212c583f8.png"
      }
    ],
    "legacyApplications": [
      {
        "applicationName": "Kaltura Login - Prod",
        "applicationId": "cb394386275e4a0b90b5cc6e77e55682"
      },
      {
        "applicationName": "Phoenix Labs",
        "applicationId": "5d6f8ef478c6490dbca8d80b27296897"
      }
    ]
  }
}
```