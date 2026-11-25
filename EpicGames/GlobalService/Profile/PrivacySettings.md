## Global Service - Profile: Get Privacy Settings

URL: https://global-profile-service.game-social.epicgames.com/profile/privacy_settings <br/>
Method: PUT <br/>
Auth Required: Yes (No Perm required)

```json
{
  "namespace": "Fortnite"
}
```

## Parameters

`namespace`: e.g. `Fortnite`

---

*Example Response*

```json
{
  "privacySettings": {
    "playRegion": "PRIVATE",
    "badges": "FRIENDS_ONLY",
    "languages": "PUBLIC"
  }
}
```
