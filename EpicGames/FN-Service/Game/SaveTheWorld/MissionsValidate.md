## FN Service - Validate STW Missions

URL: https://fngw-mcp-gc-livefn.ol.epicgames.com/fortnite/api/game/v2/world/validate <br/>
Method: POST <br/>
Auth Required: Yes (`fortnite:fortnite_role:dedicated_server ALL`)

```json
{
    "worldId": "",
    "theaterId": "8633333E41A86F67F78EAEAF25BF4735",
    "theaterMissionId": "b9c086b0-d157-446b-b52c-0648752201d3",
    "theaterMissionAlertId": "",
    "zoneThemeClass": "/Game/World/ZoneThemes/Onboarding/ZT_OnboardingFort/BP_ZT_Onboarding_Fort.BP_ZT_Onboarding_Fort_C"
}
```

## Query Parameters

`sessionId`: The sessionId to validate

---

*Example Response (Mission is Valid)*

```json
{
    "worldId": "",
    "theaterId": "8633333E41A86F67F78EAEAF25BF4735",
    "theaterMissionId": "b9c086b0-d157-446b-b52c-0648752201d3",
    "theaterMissionAlertId": "",
    "zoneThemeClass": "/Game/World/ZoneThemes/Onboarding/ZT_OnboardingFort/BP_ZT_Onboarding_Fort.BP_ZT_Onboarding_Fort_C"
}
```
