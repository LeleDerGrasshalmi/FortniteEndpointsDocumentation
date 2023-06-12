## Launcher Service - Assets: Check Launcher Version

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/info/launcher/:version \
Method: GET \
Auth Required: Yes (`buildinfo:buildmanifest:app:EpicGamesLauncher:build:{version}:status READ`)

## Path Parameters

`version`: Your Launcher Version, e.g. `15.4.0-25591319+++Portal+Release-Live-Windows`

---

_Example Response_ - `2.9.2-2874913+++Portal+Release-Live-Windows`

```json
{
  "status": "DEPRECATED"
}
```

_Example Response_ - `15.4.0-25591319+++Portal+Release-Live-Windows`

```json
{
  "status": "NOT_DEPRECATED"
}
```
