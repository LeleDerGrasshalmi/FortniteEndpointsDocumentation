## PRM Dialog Service - Fortnite BR: MOTD

URL: https://prm-dialogue-public-api-prod.edea.live.use1a.on.epicgames.com/api/v1/fortnite-br/surfaces/motd/target \
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

> `Not gonna explain every Parameter, they are obvious when you look at the key.` <br/>
> Those are not all Parameters that exist and im not updating this list every Update / Season... <br/>
> But \*recently Epic added the Account needs to actually play to see latest news instead if something like seasons defaults.

\*recently: ~December 2022

---

_Example Response (shortened)_

```json
{
  "contentType": "collection-with-metadata",
  "contentId": "motd-default-collection",
  "tcId": "f111d6e2-384d-4761-9ba6-c8b4930f5d36",
  "contentItems": [
    {
      "contentType": "content-item",
      "contentId": "1b707fac-57b1-468c-8248-6773bca2858a",
      "tcId": "b79859d8-b4e3-4f1f-8bd2-ea1ce564c945",
      "contentFields": {
        "body": "Seek training and learn to use the Force to push, pull, or lift objects and players! Force training allows you to sprint faster and double jump while a Lightsaber is equipped.",
        "buttonTextOverride": "Play Now",
        "category": "set_br_playlists",
        "entryType": "Text",
        "image": [
          {
            "width": 1920,
            "height": 1080,
            "url": "https://cdn-live.prm.ol.epicgames.com/prod/6656c2f3f18687d38a71568357005a6045ede0966091265f347d397637a6b2b5335ab02be2e32424d8cb4e5129a439c03dc5b45b4e9a04fc412fcd52d15898eb-3f37050d-8fba-4eb4-91ea-0f900b304972.jpeg?width=1920"
          }
        ],
        "islandCode": "set_br_playlists",
        "tabTitleOverride": "Force Abilities",
        "tileImage": [
          {
            "width": 1024,
            "height": 512,
            "url": "https://cdn-live.prm.ol.epicgames.com/prod/6656c2f3f18687d38a71568357005a6045ede0966091265f347d397637a6b2b596a64b38938e3bba211c57dd2e3818d7-239028aa-1480-46c6-abe5-c6232f458ba5.jpeg?width=1024"
          }
        ],
        "title": "Force Abilities",
        "videoAutoplay": false,
        "videoStreamingEnabled": true,
        "videoUID": "xfrwDSOkjtfKpTCwHg",
        "videoVideoString": "StarWars_EngagementEvent_GameplayTrailer"
      },
      "contentSchemaName": "DiscoveryMotd"
    }
  ],
  "metadata": {
    "contentType": "content-item",
    "contentId": "2b89f387-cc8b-473a-8fa3-87891c38570b",
    "tcId": "031237c8-9639-4f01-99d2-81081bf2b159",
    "contentFields": {
      "autoOpen": false
    },
    "contentSchemaName": "Metadata"
  }
}
```
