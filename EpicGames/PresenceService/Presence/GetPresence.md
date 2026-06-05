## Presence Service - Get Presence

URL: https://presence-public-service-prod.ol.epicgames.com/presence/api/v1/_/:accountId/presence \
Method: GET \
Auth Required: Yes (`presence:_:{accountId} READ`)

## Path Parameters

`accountId`: Your AccountId

## Query Parameters

`circle`: Specify the returned data, `self` (default) and `friends` are valid, can be combined when using the query multiple times

---

_Example Response_

```json
[
  {
    "circle": "self",
    "presences": [
      {
        "accountId": "94b1569506b04f9f8557af611e8c5e47",
        "status": "away",
        "perNs": [
          {
            "productId": "prod-fn",
            "appId": "fghi4567FNFBKFz3E4TROb0bmPS8h1GW",
            "status": "away",
            "activity": {},
            "ns": "62a9473a2dca46b29ccf17577fcf42d7",
            "props": {
              "SessionIdAttributeKey": "s85ab0dbfd1034a3db92f01d5694cbd22",
              "IslandCode": "scampaign",
              "FortPartySize": "i1",
              "InUnjoinableMatch": "bfalse",
              "EOS_ProductName": "Fortnite",
              "EOS_IntegratedPlatform": "EGS",
              "EOS_ProductVersion": "++Fortnite+Release-40.41-CL-54326946",
              "FortBasicInfo": "m{\"homeBaseRating\":32}",
              "EOS_Lobby": "{\"version\":3}",
              "FortLFG": "i0",
              "EOS_OnlinePlatformType": "100",
              "FortSubGame": "i0",
              "FortGameplayStats": "m{\"state\":\"\",\"playlist\":\"None\",\"numKills\":0,\"bFellToDeath\":false}",
              "EOS_Session": "{\"version\":3}",
              "IsInZone": "bfalse",
              "SocialStatus": "m{\"attendingSocialEventIds\":[]}",
              "EOS_Platform": "WIN",
              "party.joininfodata.286331153": "m{\"bIsPrivate\":true}"
            },
            "conns": [
              {
                "id": "daded2fffe2ec20a-00000001-0121e40d-8a47f2e8c5737cd3-fca21827#sub-eas-4167271840",
                "props": {}
              }
            ]
          }
        ]
      }
    ]
  },
  {
    "circle": "friends",
    "presences": [
      {
        "accountId": "db23dfc6b0e34a81808648d9277935ac",
        "status": "xa",
        "perNs": [
          {
            "productId": "prod-fn",
            "appId": "fghi4567FNFBKFz3E4TROb0bmPS8h1GW",
            "status": "xa",
            "activity": {
              "value": "Rette die Welt: Twine Peaks (140)"
            },
            "ns": "62a9473a2dca46b29ccf17577fcf42d7",
            "props": {
              "Event_PartySize": "s5",
              "SessionIdAttributeKey": "s88872af64495497194c6afe58a12d822",
              "IslandCode": "scampaign",
              "FortPartySize": "i1",
              "SocialStatus": "m{\"attendingSocialEventIds\":[]}",
              "EOS_ProductName": "Fortnite",
              "EOS_IntegratedPlatform": "EGS",
              "EOS_ProductVersion": "++Fortnite+Release-40.41-CL-54326946",
              "FortBasicInfo": "m{\"homeBaseRating\":145}",
              "GamePlaylistName": "sPlaylist_VK_Play",
              "Event_PartyMaxSize": "s16",
              "EOS_Lobby": "{\"version\":3}",
              "EOS_OnlinePlatformType": "100",
              "FortLFG": "i0",
              "FortGameplayStats": "m{\"state\":\"\",\"playlist\":\"None\",\"numKills\":0,\"bFellToDeath\":false}",
              "FortSubGame": "i0",
              "Event_PlayersAlive": "s4",
              "EOS_Session": "{\"version\":3}",
              "IsInZone": "bfalse",
              "EOS_Platform": "WIN",
              "InUnjoinableMatch": "bfalse",
              "party.joininfodata.286331153": "m{\"bIsPrivate\":true}"
            },
            "conns": [
              {
                "id": "52f80cfffe097b6c-00000001-00fcc646-c43cbda714d7fcb8-1dd58190#sub-eas-3820647448",
                "props": {}
              }
            ]
          }
        ]
      },
      {
        "accountId": "5f38c3127c8f44f9b59ae33b095d60b0",
        "status": "online",
        "perNs": [
          {
            "status": "online",
            "ns": "_",
            "props": {
              "bIsPlaying": "false",
              "bIsJoinable": "false",
              "SessionId": "",
              "bHasVoiceSupport": "false"
            },
            "conns": [
              {
                "id": "6ab6e3fffeab4dac-00000001-000fa3e4-4813f79cbd9983b3-90d5ddeb",
                "runningApp": {
                  "id": "879b0d8776ab46a59a129983ba78f0ce",
                  "displayName": "Genshin Impact"
                },
                "props": {
                  "running_app_name": "Genshin Impact",
                  "running_app_id": "879b0d8776ab46a59a129983ba78f0ce"
                }
              },
              {
                "id": "7ee917fffee20702-00000001-0063b26f-55c95a57164d93cc-7b968a8b",
                "props": {}
              }
            ]
          }
        ]
      }
    ]
  }
]
```
