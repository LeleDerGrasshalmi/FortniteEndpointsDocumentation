## PRM Dialog Service - Fortnite BR: Dynamic MOTD

URL: https://prm-dialogue-public-api-prod.edea.live.use1a.on.epicgames.com/api/v1/fortnite-br/surfaces/dmotd/target \
Method: POST \
Auth Required: Yes (Account - `eg1`)

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

> Apparently the params as [Motd request](./MOTD.md)

---

_Example Response (shortened)_

```json
{
  "contentType": "collection",
  "contentId": "fortnite-br-dmotd-collection",
  "tcId": "ee5cfa79-7850-412e-8de4-8c8346d0574e",
  "contentItems": [
    {
      "contentType": "content-item",
      "contentId": "daa34ea0-bded-44ea-ab3b-863b2992ef22",
      "tcId": "fabfac02-328c-434a-afc6-fe89ea4e2866",
      "contentFields": {
        "FullScreenBackground": {
          "Image": [
            {
              "width": 1920,
              "height": 1080,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/ed2995a8389807324b3b6c8c124d4285ff1217ad85c8f3f6d0a715dbf781b300cd17a8a44f614fc07ec3a7626bbc1e08-f77b3299-f20f-4fcc-b3f5-68a96d0653f6.jpeg?width=1920"
            },
            {
              "width": 960,
              "height": 540,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/ed2995a8389807324b3b6c8c124d4285ff1217ad85c8f3f6d0a715dbf781b300cd17a8a44f614fc07ec3a7626bbc1e08-f77b3299-f20f-4fcc-b3f5-68a96d0653f6.jpeg?width=960"
            }
          ],
          "_type": "FullScreenBackground"
        },
        "FullScreenBody": "Complete Fortnitemares Quests to earn sweet cosmetic rewards, bite back with the Wood Stake Shotgun, defeat Kado Thorne to wield his Vampiric Blade and more until November 3.",
        "FullScreenTabTitle": "Fortnitemares",
        "FullScreenTitle": "Fortnitemares",
        "TeaserBackground": {
          "Image": [
            {
              "width": 1024,
              "height": 512,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/ed2995a8389807324b3b6c8c124d4285f8e1cb11d8e38104a340d1a7d7c1f4aa498c09801dff6b1f7e0a05e206705f5f-d0824304-95d8-4278-9929-351b4a157600.jpeg?width=1024"
            }
          ],
          "_type": "TeaserBackground"
        },
        "TeaserTitle": "Fortnitemares"
      },
      "contentSchemaName": "DynamicMotd",
      "contentHash": "ddea95d7eb05d34865471c84bf6156b7"
    },
    {
      "contentType": "content-item",
      "contentId": "b0a5c01e-c525-4981-b587-07d0bb61264c",
      "tcId": "afcd3051-6919-4c1c-9dd9-2467895d0dd4",
      "contentFields": {
        "FullScreenBackground": {
          "Image": [
            {
              "width": 1920,
              "height": 1080,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/e519db5f39da339157e50a902698b3cf1d80285aa6bde1e0c2a15a7344af89de9f3be01468f8cb388e78ac78e4c2b687-5aa548a7-9baa-4754-b3af-b0fb1281dd29.jpeg?width=1920"
            },
            {
              "width": 960,
              "height": 540,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/e519db5f39da339157e50a902698b3cf1d80285aa6bde1e0c2a15a7344af89de9f3be01468f8cb388e78ac78e4c2b687-5aa548a7-9baa-4754-b3af-b0fb1281dd29.jpeg?width=960"
            }
          ],
          "_type": "FullScreenBackground"
        },
        "FullScreenBody": "Meet the ultimate heist team led by maverick Nolan Chance, bring the muscle with Fish Thicc, strike back with Jedi warrior Ahsoka Tano and more!",
        "FullScreenTabTitle": "Battle Pass",
        "FullScreenTitle": "Battle Pass",
        "TeaserBackground": {
          "Image": [
            {
              "width": 1024,
              "height": 512,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/e519db5f39da339157e50a902698b3cf73ddf599ecd711cac40afd09639c3a5b61c08bfe8e38ef2f04ced6d1f0d4b5d2-e2f82ea1-1106-4c18-bc96-91194eaa3778.jpeg?width=1024"
            }
          ],
          "_type": "TeaserBackground"
        },
        "TeaserTitle": "Battle Pass"
      },
      "contentSchemaName": "DynamicMotd",
      "contentHash": "8d28aa8aba21b0a515dabc7c4d9b7b5a"
    },
    {
      "contentType": "content-item",
      "contentId": "03a170f3-74b8-44e0-83de-0bf5d7e7edbe",
      "tcId": "67ba0f94-2c3d-457c-bf93-1e989730b99b",
      "contentFields": {
        "FullScreenBackground": {
          "Image": [
            {
              "width": 1920,
              "height": 1080,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/80c817c5763f5d123319e1237589d9de9fadefeedc7391003463cd47ea06e861363f94cf08bec61c1c12ff8b2e817030679df4ea2208a2af1e68a54e0d37c6c1-a3cedaf6-a0d5-4b36-a9b7-99229257f0e2.jpeg?width=1920"
            },
            {
              "width": 960,
              "height": 540,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/80c817c5763f5d123319e1237589d9de9fadefeedc7391003463cd47ea06e861363f94cf08bec61c1c12ff8b2e817030679df4ea2208a2af1e68a54e0d37c6c1-a3cedaf6-a0d5-4b36-a9b7-99229257f0e2.jpeg?width=960"
            }
          ],
          "_type": "FullScreenBackground"
        },
        "FullScreenBody": "A shotgun that’s not afraid to bite back.",
        "FullScreenTabTitle": "Wood Stake Shotgun",
        "FullScreenTitle": "Wood Stake Shotgun",
        "TeaserBackground": {
          "Image": [
            {
              "width": 1024,
              "height": 512,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/80c817c5763f5d123319e1237589d9de9fadefeedc7391003463cd47ea06e8616bb6992ff82facf90f179df7275f47fde8deaffbd6551d6e0bfa927c8811f12d-20e31c13-7de9-4df9-927d-bb3444333adc.jpeg?width=1024"
            }
          ],
          "_type": "TeaserBackground"
        },
        "TeaserTitle": "Wood Stake Shotgun"
      },
      "contentSchemaName": "DynamicMotd",
      "contentHash": "d769e432865cdde7f3937348b8b8a5ca"
    },
    {
      "contentType": "content-item",
      "contentId": "37617e7d-7ba0-4990-a406-2fb22a5fe3eb",
      "tcId": "acecdc31-e04a-4cea-a09f-ccacfcfcd7d1",
      "contentFields": {
        "FullScreenBackground": {
          "Image": [
            {
              "width": 1920,
              "height": 1080,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/9e741b3e1037837ae87ebedf05ec63b9e309ab654f688011e4b49ae49bf72f011c8e43c4fc5943e05b8170304bd13bfccf533ed826375408b34e2669ab65b986-e21d77c6-5ed3-4080-834f-ee540e2307fd.jpeg?width=1920"
            },
            {
              "width": 960,
              "height": 540,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/9e741b3e1037837ae87ebedf05ec63b9e309ab654f688011e4b49ae49bf72f011c8e43c4fc5943e05b8170304bd13bfccf533ed826375408b34e2669ab65b986-e21d77c6-5ed3-4080-834f-ee540e2307fd.jpeg?width=960"
            }
          ],
          "_type": "FullScreenBackground"
        },
        "FullScreenBody": "Complete Fortnitemares Quests until November 3 to earn cosmetic rewards, including the Bat Royale Back Bling, the Hypo-Bat Spray and the Revenant Rider Glider.",
        "FullScreenTabTitle": "Fortnitemares Quests",
        "FullScreenTitle": "Fortnitemares Quests",
        "TeaserBackground": {
          "Image": [
            {
              "width": 1024,
              "height": 512,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/9e741b3e1037837ae87ebedf05ec63b9e309ab654f688011e4b49ae49bf72f01d4fcab0ce79d9300d396ae0c2359a5e16f1c96832fb53faf969c54e72487be6a-e958f7cf-fe79-4e3a-8739-2162fe58847e.jpeg?width=1024"
            }
          ],
          "_type": "TeaserBackground"
        },
        "TeaserTitle": "Fortnitemares Quests"
      },
      "contentSchemaName": "DynamicMotd",
      "contentHash": "302158d457d28e656cba16e9eaf660b7"
    },
    {
      "contentType": "content-item",
      "contentId": "bce546e1-d9ca-42ae-a2e2-e4a9ee40cefb",
      "tcId": "6095e2c6-dde2-405e-8a67-e582f5f588eb",
      "contentFields": {
        "FullScreenBackground": {
          "Image": [
            {
              "width": 1920,
              "height": 1080,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/d6e7211ba391caa7ee0c9051c1a49b5411861fb2ff609b462375135840079d7f560e862b15d285fd0413b540d6738a2afa05c87fcb8d13f1b9e88563b61532f4-6a50f790-a4c2-4b16-8572-9b55b13a83fe.jpeg?width=1920"
            },
            {
              "width": 960,
              "height": 540,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/d6e7211ba391caa7ee0c9051c1a49b5411861fb2ff609b462375135840079d7f560e862b15d285fd0413b540d6738a2afa05c87fcb8d13f1b9e88563b61532f4-6a50f790-a4c2-4b16-8572-9b55b13a83fe.jpeg?width=960"
            }
          ],
          "_type": "FullScreenBackground"
        },
        "FullScreenBody": "The FNCS Global Championship is coming in three days. Jump into Legends Landing on October 13 and watch some of the best competitive players compete for the FNCS champions crown. More info: fn.gg/GC2023",
        "FullScreenTabTitle": "FNCS Global Championship",
        "FullScreenTitle": "FNCS Global Championship",
        "TeaserBackground": {
          "Image": [
            {
              "width": 1024,
              "height": 512,
              "url": "https://cdn-live.prm.ol.epicgames.com/prod/d6e7211ba391caa7ee0c9051c1a49b5411861fb2ff609b462375135840079d7fcbe5af3d9ac1702c3ce1289eccba7578cb894ab3c7fe583a831397f3a1b5dde1-1dd734db-4021-443c-89fd-54031c7badc3.jpeg?width=1024"
            }
          ],
          "_type": "TeaserBackground"
        },
        "TeaserTitle": "FNCS Global Championship"
      },
      "contentSchemaName": "DynamicMotd",
      "contentHash": "5af8aa4c91af291bac2af3eeac9a55fe"
    }
  ]
}
```
