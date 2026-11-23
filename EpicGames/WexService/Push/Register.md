## Wex Service - Push Notification: Register Device

URL: https://wex-public-service-live-prod.ol.epicgames.com/wex/api/push/:accountId/register <br/>
Method: POST <br/>
Auth Required: Yes (`wexp:push:devices:{accountId} CREATE`)

## Path Parameters

`accountId`: The account ID to register the device for

## Query Parameters

`deviceToken`: The device token to register with <br/>
`platform`: The platform of the device e.g. `ANDROID` <br/>
`locale`: The locale of the device e.g. `en-AU` <br/>
`tzOffset`: The timezone offset of the device e.g. `10` <br/>
`rvn`: The profile0 revision number e.g. `40532`

---

*Example Response*

> Unknown
