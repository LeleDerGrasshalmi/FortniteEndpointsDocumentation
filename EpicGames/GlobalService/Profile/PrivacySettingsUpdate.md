## Global Service - Profile: Modify Privacy Settings

URL: https://global-profile-service.game-social.epicgames.com/profile/privacy_settings \
Method: POST \
Auth Required: Yes (No Perm required)

```json
{
  "namespace": "",
  "privacy_settings": {
    "playRegion": "",
    "languages": "",
    "badges": ""
  }
}
```

## Parameters

`namespace`: e.g. `Fortnite` \
`playRegion` / `languages` / `badges`:

- PUBLIC
- FRIENDS_ONLY
- PRIVATE
