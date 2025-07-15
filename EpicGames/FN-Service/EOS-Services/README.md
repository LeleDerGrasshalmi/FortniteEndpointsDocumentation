# FN - EOS Services Authentication

**_These APIs require EOS Connect authentication, an example how to get such an token is shown below._** <br/>
_Therefore the permission(s) listed in the requests are policy permissions, not client permissions (thats how EOS works)_

---

URL: https://api.epicgames.dev/auth/v1/oauth/token \
Method: POST \
Auth Required: Yes (Basic Authentication where the username is the Client Id and the password is the Client Secret)

## Headers

`Content-Type`: application/x-www-form-urlencoded

## Parameters

`grant_type`: `external_auth` <br/>
`external_auth_type`: `epicgames_access_token` <br/>
`external_auth_token`: Your normal epic games access token (EG1, Opaque, EAS) <br/>
`deployment_id`: The Deployment Id from env configuration, for `live-fn` it is `62a9473a2dca46b29ccf17577fcf42d7` <br/>
`nonce`: Random nonce string

---

_Example Response_

```json
{
  "access_token": "REDACTED",
  "token_type": "bearer",
  "expires_at": "2025-07-15T19:44:49.812Z",
  "nonce": "_",
  "features": [
    "AntiCheat",
    "Connect",
    "ContentService",
    "Ecom",
    "EpicConnect",
    "Inventories",
    "LockerService",
    "Matchmaking Service",
    "PCBService",
    "QuestService"
  ],
  "organization_id": "o-aa83a0a9bc45e98c80c1b1c9d92e9e",
  "product_id": "prod-fn",
  "sandbox_id": "fn",
  "deployment_id": "62a9473a2dca46b29ccf17577fcf42d7",
  "organization_user_id": "000135c3d47e4198a91a01320374fd4d",
  "product_user_id": "0002968544584824a0c528dad8b75bf9",
  "product_user_id_created": false,
  "id_token": "REDACTED",
  "expires_in": 3599
}
```

---

Example plain http request sent by the game

```http
POST https://api.epicgames.dev/auth/v1/oauth/token HTTP/1.1
Host: api.epicgames.dev
Accept-Encoding: identity
Content-Type: application/x-www-form-urlencoded
Accept: application/json
Authorization: Basic ZWM2ODRiOGM2ODdmNDc5ZmFkZWEzY2IyYWQ4M2Y1YzY6ZTFmMzFjMjExZjI4NDEzMTg2MjYyZDM3YTEzZmM4NGQ=
X-Epic-Correlation-ID: EOS-REDACTED
User-Agent: EOS-SDK/1.16.3000-33300249 (Windows/10.0.19041.4165.64bit) Fortnite/++Fortnite+Release-30.00-CL-33962396
X-EOS-Version: 1.16.3000-33300249

grant_type=external_auth&external_auth_type=epicgames_access_token&external_auth_token=REDACTED&deployment_id=62a9473a2dca46b29ccf17577fcf42d7&nonce=REDACTED
```
