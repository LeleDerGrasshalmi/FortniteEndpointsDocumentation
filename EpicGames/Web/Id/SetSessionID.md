## Id Web - Set Session ID

URL: https://www.epicgames.com/id/api/set-sid?sid=:sid \
Method: GET \
Auth Required: No

## Query Parameters

`sid`: The Session ID grabbed from [AuthorizationCode](https://github.com/LeleDerGrasshalmi/FortniteEndpointsDocumentation/blob/main/EpicGames/Web/Id/Auth/AuthorizationCode.md) when not specifying a responseType

---

_Example Response Status: 204 (No Content)_

_Example Response Status (Session ID is invalid)_

```json
{
    "errorCode": "errors.com.epicgames.accountportal.session_id_invalid",
    "message": "Session ID is invalid or expired.",
    "correlationId": "00000000-0000-0000-0000-000000000000"
}
```
