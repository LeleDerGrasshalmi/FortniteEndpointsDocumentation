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

## Parameters

`flow`: (optional), The Device Code Flow Type, one of `login`, `register` or `quick` <br/>
`dateOfBirth`: (optional), The Birthdate, e.g. `2022-10-31` <br/>
`prompt`: (optional), The Device Code Promt, one of `none`, `login`, `new_session`, `register`, `consent`, `pass_through`, `2nd_domain`, `upgrade`, `skip_upgrade`, `skip_merge`, `activate` <br/>
`continuation`: (optional), The Continuation Token

---

_Example Response_

```json
{
  "userCode": "CVHWRDPZ",
  "expiresIn": 600,
  "interval": 10,
  "verificationUri": "https://www.epicgames.com/activate"
}
```
