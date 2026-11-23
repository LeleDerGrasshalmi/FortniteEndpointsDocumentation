## Id Web - Login

URL: https://www.epicgames.com/id/api/login <br/>
Method: POST <br/>
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

*Example Response (Successful)*: Status 200 (No Content)

*Example Response (Captcha or CSRF Token are invalid)*

```json
{
  "errorCode": "errors.com.epicgames.accountportal.captcha_invalid",
  "message": "Incorrect response. Please refresh the page.",
  "correlationId": "ad782d20-5d5d-11ee-8839-43f54ba607b9"
}
```
