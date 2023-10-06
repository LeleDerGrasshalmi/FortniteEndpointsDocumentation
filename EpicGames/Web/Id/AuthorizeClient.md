## Id Web - Authorize Scope for Client

URL: https://www.epicgames.com/id/api/client/:clientId/authorize \
Method: POST \
Auth Required: Yes

```json
{
  "scope": [],
  "continuation": "",
  "userCode": ""
}
```

## Path Parameters

`id`: The Id of the Client

## Parameters

`scope`: Required, list of scopes to authorize for next login <br/>
`continuation`: Optional, Continuation token used for corrective actions (supplied on login) <br/>
`userCode`: Optional, userCode used for login with the unauthorized scope 

---

_Example Response (Successful)_: Status 200 (No Content)

_Example Response (Client not allowed to use scope)_

```json
{
   "errorCode":"errors.com.epicgames.accountportal.unauthorized_scope",
   "message":"Client is not authorized to request the following scope: relevant_cosmetics.",
   "correlationId":"00000000-0000-0000-0000-000000000000"
}
```

_Example Response (Scope is invalid)_

```json
{
    "errorCode": "errors.com.epicgames.accountportal.validation.allowed",
    "message": "scope must be one of [openid, offline_access, basic_profile, friends_list, friends_management, presence, library, country, relevant_cosmetics]",
    "correlationId": "00000000-0000-0000-0000-000000000000"
}
```
