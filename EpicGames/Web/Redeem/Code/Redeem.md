## Redeem Web - Redeem

URL: https://redeem.epicgames.com/api/code/redeem \
Method: POST \
Auth Required: Yes

```json
{
    "code": "aaaaaaaaaaaaaaaa",
    "locale": "en-US",
    "solveToken": ""
}
```

## Parameters

`code`: Code to Redeem <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en-US' <br/>
`solveToken`: Final Captcha Token

---