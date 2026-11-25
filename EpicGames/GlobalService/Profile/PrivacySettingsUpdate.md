## Global Service - Profile: Modify Privacy Settings

URL: https://global-profile-service.game-social.epicgames.com/profile/privacy_settings <br/>
Method: POST <br/>
Auth Required: Yes (No Perm required)

```json
{
  "namespace": "Fortnite",
  "privacy_settings": {
    "playRegion": "PUBLIC",
    "languages": "FRIENDS_ONLY",
    "badges": "PRIVATE"
  }
}
```

## Parameters

`namespace`: e.g. `Fortnite` <br/>
`playRegion` / `languages` / `badges`:

- PUBLIC
- FRIENDS_ONLY
- PRIVATE

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
