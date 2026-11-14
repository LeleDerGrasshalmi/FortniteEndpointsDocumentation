## EULA Tracking Service - Accept Agreement

URL: https://eulatracking-public-service-prod06.ol.epicgames.com/eulatracking/api/public/agreements/:key/version/:version/account/:accountId/accept \
Method: POST \
Auth Required: Yes (Account Auth)

## Path Parameters

`key`: Agreement key, e.g. `emporium` <br/>
`version`: `version` from [Get Pending Agreement](./GetAgreement.md) <br/>
`accountId`: Your Account Id

## Query Parameters

`locale`: Language of the accepted text, e.g. `en`

---

_Example Response_: Status 204

_Example Response (unknown version)_

```json
{
  "errorCode": "errors.com.epicgames.eulatracking.agreement_not_found",
  "errorMessage": "The agreement with key emporium and version 999 could not be found.",
  "messageVars": ["emporium", "999"],
  "numericErrorCode": 31003,
  "originatingService": "com.epicgames.eulatracking",
  "intent": "prod"
}
```
