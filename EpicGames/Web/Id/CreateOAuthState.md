## Id Web - Create State for External Login

URL: https://www.epicgames.com/id/api/state \
Method: POST \
Auth Required: Yes

```json
{
  "redirectUrl": "http://localhost",
  "psnRedirectUrl": "https://sony.com",
  "oauthRedirectUrl": "http://fortnite.com",
  "isPopup": true,
  "isWeb": false,
  "steamAccountId": "1",
  "accountId": "39032a71931a4f129f01d6899da9e036",
  "loginRequestId": "39032a71931a4f129f01d6899da9e036",
  "code": "39032a71931a4f129f01d6899da9e036",
  "allowThirdParties": true,
  "parentalControls": {
    "voiceChat": "nobody",
    "textChat": "nobody"
  },
  "system": "PEGI",
  "rating": "unrated",
  "trackingUuid": "58a9874d11ae4d619e1dd98a028229c4"
}
```

## Parameters

`redirectUrl`: the redirect url receiving the state <br/>
`psnRedirectUrl`: The Playstation Network redirect url returning the state (Note: Can't be used with `oauthRedirectUrl`) <br/>
`oauthRedirectUrl`: The epic OAuth redirect url returning the state (Note: Can't be used with `psnRedirectUrl`) <br/>
`isPopup`: Is the external authorization a popup? <br/>
`isWeb`: Is the external authorization a webpage? <br/>
`steamAccountId`: The steam account id authorizing using the state in authorization <br/>
`accountId`: The epic account id authorizing using the state in authorization <br/>
`loginRequestId`: Unknown for now <br/>
`code`: The [Authorization Code](https://github.com/LeleDerGrasshalmi/FortniteEndpointsDocumentation/blob/main/EpicGames/Web/Id/Auth/AuthorizationCode.md)
used for authorization <br/>
`allowThirdParties`: Should third parties use this state? <br/>
`parentalControls`: A JSON Object with parental controls <br/>
`system` Rating system used. Valid: `PEGI`, `ESRB` (Note: when using this `rating` param will become required) <br/>
`rating` The rating for the state's app. Valid for PEGI: (`pegi3`, `pegi7`, `pegi10`, `pegi12`, `pegi16`, `pegi18`, `unrated`), Valid for ESRB: (`everyone`, `everyone10`, `teen`, `mature`, `adultsOnly`, `unrated`) <br/>
`trackingUuid`: Tracking UUID grabbed from [Analytics API](https://github.com/LeleDerGrasshalmi/FortniteEndpointsDocumentation/blob/main/EpicGames/Web/Id/Analytics.md)

## Any of these Parameters are optional unless specified

_Example Response (Successful)_:

_Plain Text Response_

```
eyJpZCI6IjJmYjY2YmZkZDk4NzRmNjFhYWYyMjkwN2VmNjU3Yjg5IiwibG9naW5SZXF1ZXN0SWQiOiIzOTAzMmE3MTkzMWE0ZjEyOWYwMWQ2ODk5ZGE5ZTAzNiJ9
```
