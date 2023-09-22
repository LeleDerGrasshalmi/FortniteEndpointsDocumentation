## Account Web - Notifications: Preferences

URL: https://www.epicgames.com/account/v2/api/notifications \
Method: GET \
Auth Required: No

## Query Parameters

`formatType`: Should be `json`

---

_Example Response_

```json
{
  "success": true,
  "results": {
    "email": {
      "settingValue": true,
      "settingKey": "email"
    },
    "email:egs:announcements": {
      "settingValue": false,
      "settingKey": "email:egs:announcements"
    },
    "email:egs:newsletter": {
      "settingValue": false,
      "settingKey": "email:egs:newsletter"
    },
    "email:egs:wishlist": {
      "settingValue": false,
      "settingKey": "email:egs:wishlist"
    },
    "email:fortnite": {
      "settingValue": false,
      "settingKey": "email:fortnite"
    },
    "email:fallguys": {
      "settingValue": false,
      "settingKey": "email:fallguys"
    },
    "email:rocketleague": {
      "settingValue": false,
      "settingKey": "email:rocketleague"
    },
    "email:survey": {
      "settingValue": false,
      "settingKey": "email:survey"
    },
    "email:creatoreco:creationtools": {
      "settingValue": true,
      "settingKey": "email:creatoreco:creationtools"
    }
  }
}
```
