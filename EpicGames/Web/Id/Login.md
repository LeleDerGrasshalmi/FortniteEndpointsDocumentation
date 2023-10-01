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

`email`: Your email <br/>
`password`: Your password <br/>
`rememberMe`: If true, your sessions should last longer (no need to relogin everytime) <br/>
`captcha`: Final Captcha Token

---

_Example Response (Successful)_: Status 200 (No Content)

_Example Response (Captcha or CSRF Token are invalid)_

```json
{
  "errorCode": "errors.com.epicgames.accountportal.captcha_invalid",
  "message": "Incorrect response. Please refresh the page.",
  "correlationId": "ad782d20-5d5d-11ee-8839-43f54ba607b9"
}
```
