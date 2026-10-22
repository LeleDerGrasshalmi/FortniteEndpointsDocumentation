## Launcher Service - Assets: App Info

URL: https://launcher-public-service-prod06.ol.epicgames.com/launcher/api/public/assets/platform/:platform/label/:label/appInfo \
Method: POST \
Auth Required: Yes

```json
{
  "appKeys": [
    {
      "artifactId": "Grunt",
      "catalogId": "9d60f0d4300a407e817ce5548f12f12d",
      "sandboxId": "5b325322a4c04b9e9e780b9a1e9b2d70"
    }
  ]
}
```

## Path Parameters

`platform`: See [Platforms](../README.md#data) <br/>
`label`: The label, usually `Live`

## Parameters

`appKeys`: Can contain multiple entries <br/>
`appKeys[].artifactId`: The App Name (from Catalog Item) <br/>
`appKeys[].catalogId`: The Catalog-Item Id <br/>
`appKeys[].sandboxId`: The Catalog Namespace

---

_Example Response_

```json
[
  {
    "appName": "Grunt",
    "labelName": "Live-Windows",
    "buildVersion": "1.2-aeeb6200374fc01a6a51c3006846a350febeb243.21-Win",
    "catalogItemId": "9d60f0d4300a407e817ce5548f12f12d",
    "namespace": "5b325322a4c04b9e9e780b9a1e9b2d70",
    "assetId": "Grunt"
  }
]
```

_Example Response (400, body without `appKeys`)_

```json
{
  "errorCode": "errors.com.epicgames.launcher.bad_argument",
  "errorMessage": "Please check the request. Required request.appKeys are missed.",
  "messageVars": [],
  "numericErrorCode": 30016,
  "originatingService": "launcher-service",
  "intent": "prod"
}
```

_Example Response (400, body is an array)_

```json
{
  "errorCode": "errors.com.epicgames.common.json_mapping_error",
  "errorMessage": "Json mapping failed.",
  "numericErrorCode": 1019,
  "originatingService": "launcher-service",
  "intent": "prod"
}
```
