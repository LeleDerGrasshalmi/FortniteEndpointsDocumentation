## Account Web - Authorized Apps

URL: https://www.epicgames.com/account/v2/authorized-apps \
Method: GET \
Auth Required: Yes

---

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
      }
    ]
  }
}
```
