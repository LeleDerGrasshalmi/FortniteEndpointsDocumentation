## FN - Content API - Content for Key

URL: https://fortnitecontent-website-prod07.ol.epicgames.com/content/api/pages/:key \
Method: GET \
Auth Required: No

## Path Parameters

`key`: Use 'fortnite-game' for Fortnite Content or 'fortnite-editor' for UEFN Content

## Query Parameters

`lang` - language of the response (e.g. 'en')

---

_Example Response (fortnite, heavily shortened)_

```json
{
  "_title": "Fortnite Game",
  "_activeDate": "2017-08-30T03:20:48.050Z",
  "lastModified": "2023-05-18T21:44:16.467Z",
  "_locale": "en-US",
  "_templateName": "blank",
  "dynamicbackgrounds": {
    "backgrounds": {
      "backgrounds": [
        {
          "backgroundimage": "https://cdn2.unrealengine.com/ch4s2-lobbyupdate-4-20-2022-lifted-copy-3840x2160-d3a138f5f9e7.jpg",
          "stage": "default",
          "_type": "DynamicBackground",
          "key": "lobby"
        },
        {
          "backgroundimage": "https://cdn2.unrealengine.com/nocturnal-storebg-cms-1921x1081-796115fa0fc9.png",
          "stage": "defaultnotris",
          "_type": "DynamicBackground",
          "key": "vault"
        }
      ],
      "_type": "DynamicBackgroundList"
    },
    "_title": "dynamicbackgrounds",
    "_noIndex": false,
    "_activeDate": "2023-05-02T07:30:00.000Z",
    "lastModified": "2023-05-02T13:51:18.036Z",
    "_locale": "en-US",
    "_templateName": "FortniteGameDynamicBackgrounds"
  },
  "_suggestedPrefetch": []
}
```

_Example Response (uefn, shortened)_

```json
{
  "_title": "fortnite-editor",
  "_noIndex": false,
  "_activeDate": "2020-03-28T16:49:57.422Z",
  "lastModified": "2023-08-08T10:46:47.804Z",
  "_locale": "en-US",
  "_templateName": "blank",
  "mainInfo": {
    "news": {
      "mainMessage": {
        "hidden": false,
        "_type": "CommonUI Simple Message Base(Text Link)",
        "link": "",
        "title": "Unreal Editor for Fortnite",
        "body": "Unreal Editor for Fortnite unlocks the power of the Unreal Editor for creators to publish new and diverse experiences in Fortnite. Use the links to the right to join our developer community and get started in UEFN!",
        "spotlight": false
      },
      "_type": "FortniteEditor News",
      "tileMessages": [
        {
          "image": "https://cdn2.unrealengine.com/developercommunity-465x344-665beb516b3e.png",
          "hidden": false,
          "_type": "CommonUI Simple Message Base(Text Link)",
          "link": "https://create.fortnite.com/news/fortnite-ecosystem-patch-notes-v25-30-update",
          "title": "Fortnite Ecosystem v25.30 Update",
          "spotlight": false
        },
        {
          "image": "https://cdn2.unrealengine.com/gettingstarted-465x344-a10fc39b4df8.png",
          "hidden": false,
          "_type": "CommonUI Simple Message Base(Text Link)",
          "link": "https://dev.epicgames.com/community/learning/courses/Yl6/fortnite-your-first-hour-in-uefn/yXkB/fortnite-your-first-hour-in-uefn-overview",
          "title": "Your First Hour in UEFN",
          "body": "Your first hour in UEFN",
          "spotlight": false
        }
      ]
    },
    "_title": "main-info",
    "_noIndex": false,
    "_activeDate": "2020-03-28T16:50:40.690Z",
    "lastModified": "2023-08-08T10:46:47.804Z",
    "_locale": "en-US",
    "_templateName": "FortniteEditorMain"
  },
  "_suggestedPrefetch": []
}
```
