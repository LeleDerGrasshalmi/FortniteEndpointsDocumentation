## PRM Dialog Service - Surface MOTD

URL: https://prm-dialogue-public-api-prod.edea.live.use1a.on.epicgames.com/api/v1/fortnite-br/surfaces/:surfaceId/target \
Method: POST \
Auth Required: Yes (Account - `eg1`)

> Removed as of 30.09.2024

```json
{
  "accountLevel": 0,
  "alienArtifacts": 0,
  "battlepass": false,
  "battlepassItemsClaimed": 0,
  "battlepassLevel": 1,
  "battlepassStars": 0,
  "completedQuests": [],
  "countOfDragonBalls": 0,
  "country": "DE",
  "dateLastPlayed": "1901-12-13T20:45:52.000Z",
  "dateLastPlayedArena": "1901-12-13T20:45:52.000Z",
  "dateLastPlayedSaveTheWorld": "2022-11-01T23:25:31.000Z",
  "dateLastPlayedTournament": "1901-12-13T20:45:52.000Z",
  "daysSinceLastSession": 44153.14098048611,
  "globalCash": 0,
  "isRestricted": true,
  "language": "en",
  "lifetimeWins": 0,
  "onLogin": true,
  "ownsSaveTheWorld": false,
  "platform": "Windows",
  "progressiveBackblingStage": 0,
  "seasonHoursPlayed": 0,
  "serverRegion": "EU",
  "socialTags": [],
  "stylePoints": 0,
  "subscription": false,
  "totalHoursPlayed": 0,
  "unlockedPages": 1
}
```

## Parameters

> `Not gonna explain every Parameter, they are obvious when you look at the key.` <br/>
> Those are not all Parameters that exist and im not updating this list every Update / Season... <br/>
> But \*recently Epic added the Account needs to actually play to see latest news instead if something like seasons defaults.

\*recently: ~December 2022

## Path Parameters

`surfaceId`: See [Surfaces](./README.md#surfaces)

---

_Example Response (no motd currently)_:

`Status 204`

_Example Response (shortened)_

```json
{
  "contentType": "collection",
  "contentId": "fortnite-br-br-motd-collection",
  "tcId": "a6d01bae-3853-4154-80b7-da72e01f3c6e",
  "contentMeta": "{\"7a427ff816c8321910c5b6020dd410a4\":[\"0ac665f8-24f4-4ddf-85a4-8557293aba53\"],\"303f130defae555b2621a189b09f3441\":[\"e7c01ef8-d51b-438b-b655-a5fc93530662\"],\"5532ab90cff25c1f66ca1f605cb97d11\":[\"f78c8632-0b86-4698-b204-1bac475c2c6e\"],\"03d5ea4cdbe83ece0fb9255a545fc00f\":[\"f55366b6-fd78-4b06-9ba1-0f8312453f3f\"],\"2d597ddb9dcb097166feebdf2c525bba\":[\"a8ab427d-94c9-4bfc-b06c-24d1d5bb217b\"]}",
  "contentItems": [
    {
      "contentType": "content-item",
      "contentId": "e7c01ef8-d51b-438b-b655-a5fc93530662",
      "tcId": "3db52c65-f656-42ad-8f0a-c782a2c3ed85",
      "contentFields": {
        "Buttons": [
          {
            "Action": {
              "_type": "MotdVideoAction",
              "video": {
                "Autoplay": false,
                "StreamingEnabled": true,
                "UID": "PpUSDhsQiYSNrQKlVk",
                "VideoString": "Juno_Announce_Cine",
                "_type": "Video"
              }
            },
            "Style": "0",
            "Text": "Watch Video",
            "_type": "Button"
          }
        ],
        "FullScreenBackground": {
          "Image": [
            {
              "width": 1920,
              "height": 1080,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/4f702810c2fc2d89cfcd5516c563a74acb0c9d41e4c228c59d8015eca61c49b3d764889158fd05f7b29fe7e7718f7051-213c730c-5de8-4d4b-bf28-c36cf6bd3f92.jpeg?width=1920"
            },
            {
              "width": 960,
              "height": 540,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/4f702810c2fc2d89cfcd5516c563a74acb0c9d41e4c228c59d8015eca61c49b3d764889158fd05f7b29fe7e7718f7051-213c730c-5de8-4d4b-bf28-c36cf6bd3f92.jpeg?width=960"
            }
          ],
          "_type": "FullScreenBackground"
        },
        "FullScreenBody": "The adventure is building. Get ready for the vast, open worlds of LEGO Fortnite - a new survival crafting game launching on December 7!",
        "FullScreenTabTitle": "N/A",
        "FullScreenTitle": "LEGO Fortnite December 7",
        "TeaserBackground": {
          "Image": [
            {
              "width": 1024,
              "height": 512,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/4f702810c2fc2d89cfcd5516c563a74a04c5d031ce7e06cf44e8ca85986731643e262407c3d9056ef4c6f7070b15049a-6d29328f-e8af-439c-851e-5756a5e5276d.jpeg?width=1024"
            }
          ],
          "_type": "TeaserBackground"
        },
        "TeaserTitle": "LEGO Fortnite December 7"
      },
      "contentSchemaName": "DynamicMotd",
      "contentHash": "303f130defae555b2621a189b09f3441"
    }
  ]
}
```
