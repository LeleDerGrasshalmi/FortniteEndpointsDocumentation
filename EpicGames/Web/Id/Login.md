## Id Web - Login

URL: https://www.epicgames.com/id/api/login \
Method: POST \
Auth Required: Yes

```json
{
  "email": "",
  "password": "",
  "rememberMe": true,
  "captcha": ""  
}
```

## Parameters

`email`: (string) Your email <br/>
`password`: (string) Your password <br/>
`rememberMe`: (boolean) If true, your sessions should last longer (no need to relogin everytime) <br/>
`captcha`: (string) Huge json, not possible to obtain without completing your captcha

---

_Example Response (Successful)_: Status 200 Response empty


_Example Response (Captcha or CSRF Token are invalid)_: Status 400

```json
{
    "errorCode": "errors.com.epicgames.accountportal.captcha_invalid",
    "message": "Incorrect response. Please refresh the page.",
    "correlationId": "ad782d20-5d5d-11ee-8839-43f54ba607b9"
}
```
