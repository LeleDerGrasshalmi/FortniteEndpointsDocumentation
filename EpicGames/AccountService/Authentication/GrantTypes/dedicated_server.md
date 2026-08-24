## Grant_Type: dedicated_server

Used by Dedicated Game Servers to authenticate with the backend services. Allows the server to act as a privileged service principal rather than a user account, granting administrative permissions necessary for match lifecycle management. (As name says its used for Fortnite Gameservers)

### Headers

| Header | Type | Description |
| :--- | :--- | :--- |
| `Content-Type` | `string` | Must be `application/x-www-form-urlencoded`. |
| `Authorization` | `string` | `Basic <Base64(Client_ID:Client_Secret)>` containing dedicated server credentials. |
| `User-Agent` | `string` | The user agent identifying the server build (e.g. `Fortnite/++Fortnite+Release-14.20-CL-14354056`). |

---

### Body Parameters

| Field | Type | Description |
| :--- | :--- | :--- |
| `grant_type` | `string` | Must be explicitly set to `dedicated_server`. |

---

### Expected Response

* **Status:** `200 OK`
* **Content-Type:** `application/json`

```json
{
  "access_token": "eg1~ds_token_8f31b790d9844c80b15438a2c7e09961",
  "token_type": "bearer",
  "expires_in": 14400,
  "expires_at": "2026-08-24T20:12:23.000Z",
  "client_id": "dedicatedServerClientId",
  "scope": "fortnite:fortnite_role:dedicated_server"
}
```

---

### System Integration & Scopes

Unlike player-facing grant types (e.g. `exchange_code` or `password`), this authentication flow operates without user credentials:
1. **Administrative Scope:** The returned access token is associated with the **`fortnite:fortnite_role:dedicated_server`** authority scope.
2. **Missing Properties:** The response payload does not include `accountId`, `displayName`, or `refresh_token` attributes, as the token represents a service identity.
3. **Usage:** The dedicated server attaches this token (`Authorization: bearer <access_token>`) to authenticate API requests for verifying connecting clients, updating matchmaking sessions, and reporting statistics.
