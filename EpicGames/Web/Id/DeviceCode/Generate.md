## EpicGames - Device Code: Generate

URL: https://www.epicgames.com/id/api/device \
Method: POST \
Auth Required: Yes

## Body

```json
{
    "flow": "login",
    "dateOfBirth": null,
    "prompt": null,
    "continuation": null
}
```

---

Example Response

```json
{
    "userCode": "",
    "expiresIn": 600,
    "interval": 10,
    "verificationUri": "https://www.epicgames.com/activate"
}
```