## Id Web - Create Device Code

URL: https://www.epicgames.com/id/api/device \
Method: POST \
Auth Required: Yes

```json
{
  "flow": "login",
  "dateOfBirth": null,
  "prompt": null,
  "continuation": null
}
```

---

_Example Response_

```json
{
  "userCode": "",
  "expiresIn": 600,
  "interval": 10,
  "verificationUri": "https://www.epicgames.com/activate"
}
```
