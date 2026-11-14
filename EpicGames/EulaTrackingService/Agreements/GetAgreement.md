## EULA Tracking Service - Get Pending Agreement

URL: https://eulatracking-public-service-prod06.ol.epicgames.com/eulatracking/api/public/agreements/:key/account/:accountId \
Method: GET \
Auth Required: Yes (Account Auth)

## Path Parameters

`key`: Agreement key, e.g. `epicgames_tos`, `egstore`, `emporium`, `uefn` <br/>
`accountId`: Your Account Id

## Query Parameters

`locale`: Language of the text, e.g. `en`

---

_Example Response_: Status 204 (nothing to accept)

_Example Response (pending, `body` shortened)_

```json
{
  "key": "uefn",
  "version": 12,
  "revision": 5,
  "title": "Unreal Editor for Fortnite Supplemental Terms to the Epic Games Terms of Service",
  "body": "<EULA.Header>1.\tIntroduction.</>\n\nUnreal Editor for Fortnite (“<EULA.Highlight>UEFN</>”) is a creation tool ...",
  "locale": "en",
  "createdTimestamp": "2026-02-27T00:03:11.840Z",
  "lastModifiedTimestamp": "2026-02-27T00:03:11.840Z",
  "status": "ACTIVE",
  "description": "EULA for Unreal Editor for Fortnite",
  "custom": false,
  "url": "https://...",
  "bodyFormat": "HTML",
  "wasDeclined": false,
  "hasResponse": false
}
```
