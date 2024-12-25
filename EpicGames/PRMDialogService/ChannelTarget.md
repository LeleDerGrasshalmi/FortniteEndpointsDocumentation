## PRM Dialog Service - Channel MOTD

URL: https://prm-dialogue-public-api-prod.edea.live.use1a.on.epicgames.com/api/v1/fortnite-br/channel/:channelId/target \
Method: POST \
Auth Required: Yes (Account - `eg1`)

```json
{
  "parameters": {
    "platform": "Windows",
    "language": "en",
    "serverRegion": "EU",
    "country": "DE",
    "passesOwned": [],
    "levelPerPass": [5, 5, 3, 5],
    "hasSavedEventDate": false,
    "hasAttendedEndOfSeasonS17": false,
    "subscription": false,
    "ownsSaveTheWorld": false,
    "filterRestricted": false,
    "filterConsent": false,
    "filterLimited": false,
    "allowedContentTypes": ["functional", "experience", "marketing"],
    "ratingAuthority": "USK",
    "rating": "USK_AGE_16",
    "socialTags": ["BR - Duos"],
    "battlepass": false,
    "battlepassLevel": 1,
    "accountLevel": 1066,
    "victoryCrownsRoyales": 0,
    "progressiveBackblingStage": 0,
    "S21ProgressivePhotonicStrikerPickaxe": 0,
    "completedQuests": ["RaiderPinkSherbetQuestGranted"]
  },
  "tags": ["Product.BR"]
}
```

## Parameters

`parameters`: These are personalized, there are also season specific parameters, this example above is from v30.20 with season specific params removed <br/>
`tags`: All Product Tags that motd's should be returned for. These can obtained via gameplaytags staring with `Product.`

## Path Parameters

`channelId`: `motd`

---

_Example Response (no motd currently)_:

`Status 204`

_Example Response (shortened)_

```json
{
  "tcId": "7fa7e812-f76c-4a6b-8ef5-87bb01e11f16",
  "contentItems": [
    {
      "contentHash": "14097b4aa536c1982843ca1d0aba13ce",
      "contentSchemaName": "DynamicMotd",
      "contentFields": {
        "Buttons": [
          {
            "Action": {
              "_type": "MotdNavigateToShopAction",
              "navAction": "1",
              "offerTrackingId": "/Game/Catalog/NewDisplayAssets/S30/DAv2_EID_GreatPool.DAv2_EID_GreatPool"
            },
            "Style": "0",
            "Text": "Check it Out",
            "_type": "Button"
          },
          {
            "Action": {
              "_type": "MotdVideoAction",
              "video": {
                "Autoplay": false,
                "ShouldLoop": false,
                "StreamingEnabled": true,
                "UID": "caKLXYdnYdxkwDFNor",
                "VideoString": "Stainless_Ringer_Emote",
                "_type": "Video"
              }
            },
            "Style": "1",
            "Text": "Watch Video",
            "_type": "Button"
          }
        ],
        "FullScreenBackground": {
          "Image": [
            {
              "width": 1920,
              "height": 1080,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/4ccf0f2b7c8b87d2e9a71869fd9f23bfa86429c6a29322aaaf49473b33a99ef9b2dac7f60d21f43026b37f57e1c3d018-f5bdfe7e-6035-4902-8339-c6d0ff11d075.jpeg?width=1920&height=1080&aspect=fill"
            },
            {
              "width": 960,
              "height": 540,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/4ccf0f2b7c8b87d2e9a71869fd9f23bfa86429c6a29322aaaf49473b33a99ef9b2dac7f60d21f43026b37f57e1c3d018-f5bdfe7e-6035-4902-8339-c6d0ff11d075.jpeg?width=960&height=540&aspect=fill"
            }
          ],
          "Video": {
            "Autoplay": true,
            "EndTime": 23,
            "ShouldLoop": true,
            "StartTime": 17,
            "StreamingEnabled": true,
            "UID": "caKLXYdnYdxkwDFNor",
            "VideoString": "Stainless_Ringer_Emote",
            "_type": "Video"
          },
          "_type": "FullScreenBackground"
        },
        "FullScreenBody": "Ring the bell and turn heads with the Ringer Emote, featuring Metallica.",
        "FullScreenTitle": "Ringer Emote",
        "TeaserBackground": {
          "Image": [
            {
              "width": 720,
              "height": 400,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/4ccf0f2b7c8b87d2e9a71869fd9f23bfcc15de91a12e3e9d9a5c98494c6df12f778927380474a909094b0f64fe1dc521-04ccdbb4-08cc-4ccb-8146-8258ea5037e8.jpeg?width=720&height=400&aspect=fill"
            }
          ],
          "Video": {
            "Autoplay": true,
            "EndTime": 23,
            "ShouldLoop": true,
            "StartTime": 17,
            "StreamingEnabled": true,
            "UID": "caKLXYdnYdxkwDFNor",
            "VideoString": "Stainless_Ringer_Emote",
            "_type": "Video"
          },
          "_type": "TeaserBackground"
        },
        "TeaserTitle": "Ringer Emote",
        "VerticalTextLayout": false
      },
      "placements": [
        {
          "trackingId": "839328d9-3c7f-4862-b988-b38da12ac019",
          "tag": "Product.Sparks",
          "position": 0
        },
        {
          "trackingId": "c3037d3f-a9f2-4f10-825d-8582d43c4ba2",
          "tag": "Product.BR",
          "position": 0
        }
      ]
    },
    {
      "contentHash": "c1260f3dd62ef150b9bd5836a303dd9f",
      "contentSchemaName": "DynamicMotd",
      "contentFields": {
        "Buttons": [
          {
            "Action": {
              "DummyField": "0",
              "_type": "MotdDiscoverySearchAction"
            },
            "Style": "0",
            "Text": "Check it out",
            "_type": "Button"
          }
        ],
        "FullScreenBackground": {
          "Image": [
            {
              "width": 1920,
              "height": 1080,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/f4acb80fca39f6a5f388ec562be9ebcd85d58be1647ab4171c5bd8a345b4bf1f-b67e6106-90dd-456f-8aea-a20514c6c91b.jpeg?width=1920&height=1080&aspect=fill"
            },
            {
              "width": 960,
              "height": 540,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/f4acb80fca39f6a5f388ec562be9ebcd85d58be1647ab4171c5bd8a345b4bf1f-b67e6106-90dd-456f-8aea-a20514c6c91b.jpeg?width=960&height=540&aspect=fill"
            }
          ],
          "_type": "FullScreenBackground"
        },
        "FullScreenBody": "It’s easier than ever to find islands in Discover! Find fun games and genres for you and your friends by searching for islands with island code, island name or tags.",
        "FullScreenTitle": "Search in Discover",
        "TeaserBackground": {
          "Image": [
            {
              "width": 720,
              "height": 400,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/f4acb80fca39f6a5f388ec562be9ebcd5a2d464cc1b04650564abff2e6e69ac0-f60bfb4b-8ae0-4072-9b7a-f69659e07776.jpeg?width=720&height=400&aspect=fill"
            }
          ],
          "_type": "TeaserBackground"
        },
        "TeaserTitle": "Search in Discover",
        "VerticalTextLayout": false
      },
      "placements": [
        {
          "trackingId": "a6e2cd88-52c6-42e8-9310-d60101031863",
          "tag": "Product.BR",
          "position": 4
        }
      ]
    }
  ],
  "combinedContentHash": "dc1084018acc5f4e00b4e9fdea40adec",
  "analyticsEventsSendingActions": [{}, {}]
}
```
