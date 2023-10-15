## Id Web - Validate State for External Login

URL: https://www.epicgames.com/id/api/state/:state \
Method: GET 


## Path Parameters

`state`: Received state from redirect

---

_Example Response (Successful)_:

```json
{
   "isPopup":false,
   "isWeb":true,
   "oauthRedirectUrl":"https://epicgames.com/id/login/steam?prompt=",
   "ip":"77.244.41.193",
   "origin":"epicgames",
   "id":"a9b8946a25124925a7f74a47d8b66f51"
}
```

_Example Response (State is invalid)_

```json
{
   "errorCode":"errors.com.epicgames.accountportal.oauth_state_invalid",
   "message":"There was an error logging you in, please try again.",
   "correlationId":"00000000-0000-0000-0000-000000000000"
}
```
