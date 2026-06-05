## Presence Service - Set Presence

URL: https://presence-public-service-prod.ol.epicgames.com/presence/api/v1/:namespace/:accountId/presence/:connectionId \
Method: GET \
Auth Required: Yes (`presence:{namespace}:{accountId} UPDATE`)

> Also available on eos under `https://api.epicgames.dev/epic/presence/v1/_:deploymentId_/:accountId/presence/:connectionId`

## Path Parameters

`accountId`: Your AccountId
`namespace`: The presence namespace, ex. `_` (launcher) or the deployment id
`connectionId`: Your Connection ID (XMPP/EOS Connect Stomp)

---

_Example Response_

```json
{
  "own": {
    "accountId": "94b1569506b04f9f8557af611e8c5e47",
    "status": "online",
    "perNs": [
      {
        "status": "online",
        "activity": {
          "value": "Lobby - 1 / 16"
        },
        "ns": "Fortnite",
        "props": {
          "X_NonEOS_ProductName": "Fortnite"
        },
        "conns": [
          {
            "id": "V2:Fortnite:WIN::C08325DA4C406A8BBBFCA19FB3CE6694",
            "props": {}
          }
        ]
      },
      {
        "status": "online",
        "activity": {
          "value": "test status"
        },
        "ns": "_",
        "props": {
          "EOS_Platform": "WIN",
          "EOS_IntegratedPlatform": "EGS",
          "EOS_OnlinePlatformType": "100",
          "EOS_ProductVersion": "++Fortnite+Release-26.00-CL-27233190",
          "EOS_ProductName": "Fortnite",
          "EOS_Session": "{\"version\":3}",
          "EOS_Lobby": "{\"version\":3}"
        },
        "conns": [
          {
            "id": "0242acfffe110005-00000001-1146cc9d-deccdc9da4a889b5-b60167cb",
            "props": {}
          }
        ]
      },
      {
        "productId": "prod-fn",
        "appId": "fghi4567FNFBKFz3E4TROb0bmPS8h1GW",
        "status": "online",
        "activity": {
          "value": ""
        },
        "ns": "62a9473a2dca46b29ccf17577fcf42d7",
        "props": {
          "EOS_ProductVersion": "++Fortnite+Release-29.01-CL-32291970",
          "EOS_Platform": "WIN",
          "EOS_IntegratedPlatform": "EGS",
          "EOS_ProductName": "Fortnite",
          "EOS_Lobby": "{\"version\":3}",
          "EOS_OnlinePlatformType": "100",
          "EOS_Session": "{\"version\":3}"
        },
        "conns": [
          {
            "id": "0242acfffe110005-00000001-1146cc9d-deccdc9da4a889b5-b60167cb",
            "props": {}
          }
        ]
      }
    ]
  }
}
```
