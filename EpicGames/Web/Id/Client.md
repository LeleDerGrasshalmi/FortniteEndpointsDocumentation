## Id Web - Client Info

URL: https://www.epicgames.com/id/api/client/:clientId \
Method: GET \
Auth Required: No

## Path Parameters

`id`: The Id of the Client

## Query Parameters

`redirectUrl`: The redirect URL you want to lookup (Note: has to be configured with the client) <br/>
`responseType`: The responseType you want to check with the client (for non-EOS Clients: `code, eula_token` for EOS Clients: `code`)

---

_Example Response (non-EOS)_

```json
{
  "clientId": "34a02cf8f4414e29b15921876da36f9a",
  "clientName": "launcherAppClient2",
  "redirectUrl": "https://localhost/launcher/authorized",
  "internal": true,
  "mailingList": null,
  "native": false,
  "product": "default",
  "allowedScopes": [],
  "epicLoginOnly": false
}
```
_Example Response (EOS)_

```json
{
    "clientId": "3446cd72694c4a4485d81b77adbb2141",
    "clientName": "Fortnite",
    "redirectUrl": "eos.3446cd72694c4a4485d81b77adbb2141://epic/auth",
    "internal": false,
    "type": "epicId",
    "verified": true,
    "native": true,
    "product": "fortnite",
    "backgroundUrl": "https://static-assets-prod.epicgames.com/account-portal/static/static/media/fortnite_s7_bg.c08b8f1f.png",
    "platforms": [
        "ps4",
        "xbox",
        "switch",
        "pc",
        "mobile"
    ],
    "allowedScopes": [
        "basic_profile",
        "friends_list",
        "presence"
    ],
    "epicLoginOnly": false,
    "autodeskLogin": false,
    "thirdParty": true
}
```
