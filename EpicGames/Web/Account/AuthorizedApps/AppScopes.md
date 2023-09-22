## Account Web - Authorized Apps: App Scopes

URL: https://www.epicgames.com/account/v2/authorized-apps/user-scopes/application/:applicationId \
Method: GET \
Auth Required: Yes

## Path Parameters

`applicationId`: The Application Id, from [The List](./Apps.md)

---

_Example Response_

```json
{
  "success": true,
  "data": {
    "applicationId": "fghi4567ENLQNc9eFlre6btvQVrxoCQh",
    "consentStatus": "OK",
    "scopes": ["basic_profile", "friends_list", "presence"]
  }
}
```
