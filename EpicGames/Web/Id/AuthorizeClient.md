## Id Web - Authorize Scope for Client

URL: https://www.epicgames.com/id/api/client/:clientId/authorize <br/>
Method: POST <br/>
Auth Required: Yes

```json
{
  "scope": [],
  "continuation": "",
  "userCode": ""
}
```

## Path Parameters

`clientId`: The Id of the Client

## Parameters

`scope`: Required, list of scopes to authorize for next login <br/>
`continuation`: Optional, Continuation token used for corrective actions (supplied on login) <br/>
`userCode`: Optional, userCode used for login with the unauthorized scope 

---

*Example Response (Successful)*: Status 200 (No Content)

*Example Response (Client not allowed to use scope)*

```json
{
   "errorCode":"errors.com.epicgames.accountportal.unauthorized_scope",
   "message":"Client is not authorized to request the following scope: relevant_cosmetics.",
   "correlationId":"00000000-0000-0000-0000-000000000000"
}
```

*Example Response (Scope is invalid)*

```json
{
    "errorCode": "errors.com.epicgames.accountportal.validation.allowed",
    "message": "scope must be one of [openid, offline_access, basic_profile, friends_list, friends_management, presence, library, country, relevant_cosmetics]",
    "correlationId": "00000000-0000-0000-0000-000000000000"
}
```
