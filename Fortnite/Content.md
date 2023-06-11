## Fortnite - Content

URL: https://fortnitecontent-website-prod07.ol.epicgames.com/content/api/pages/fortnite-game \
Method: GET \
Auth Required: No

## Query Parameters

`lang` - language of the response (e.g. 'en')

<br/>

> Specific Data Only: <br/>
> You need to use the **\_title** Property in **lowercase** like `https://fortnitecontent-website-prod07.ol.epicgames.com/content/api/pages/fortnite-game/:_title` <br/>
> For Example we take the 'shopSections' Data, when requesting `https://fortnitecontent-website-prod07.ol.epicgames.com/content/api/pages/fortnite-game/shopSections` <br/>
> we will get status 404, but when using the `'_title' property` which is 'shop-sections' we get status 200

---

_Example Response (heavily shortened)_

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
