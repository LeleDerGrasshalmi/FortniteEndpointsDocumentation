## Id Web - Exchange Code Info

URL: https://www.epicgames.com/id/api/exchange/:exchangeCode \
Method: GET \
Auth Required: No

## Path Parameters

`exchangeCode`: The Exchange Code

---

_Example Response (Valid)_

```json
{}
```

_Example Response (Invalid)_

```json
{
  "errorCode": "errors.com.epicgames.account.oauth.single_use_code_not_found",
  "message": "Sorry, the OAuth exchange or authorization code you are using is not valid. Please try again with a new code.",
  "metadata": {},
  "correlationId": "00000000-0000-0000-0000-000000000000",
  "numericErrorCode": 18001
}
```
