## Avatar Service - Avatar Settings

URL: https://api.epicgames.dev/epic/avatar/v1/:deploymentId/accounts/:accountId/settings \
Method: GET \
Auth Required: Yes (Account Auth)

## Path Parameters

`deploymentId`: `9c9906b240c74a92a6b9100d6e4ccbd0` <br/>
`accountId`: Your Account Id (another account's id returns 403)

---

_Example Response_

```json
{
  "avatar": {
    "avatarId": "AthenaCharacter:cid_defaultoutfit[2,6]",
    "url": "https://cosmo.fdeb.live.use1a.on.epicgames.com/cdn-cgi/image/height={},format=png/v1/item/HNbvcohOxY4TnWtpDLdeUInh7V_DipmSPvrhzLo6A6I/png"
  },
  "sync": true
}
```
