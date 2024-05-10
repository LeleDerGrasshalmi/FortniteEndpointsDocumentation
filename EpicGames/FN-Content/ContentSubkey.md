## FN - Content API - Content for Subkey

URL: https://fortnitecontent-website-prod07.ol.epicgames.com/content/api/pages/:key/:subKey \
Method: GET \
Auth Required: No

## Path Parameters

`key`: Use 'fortnite-game' for Fortnite Content or 'fortnite-editor' for UEFN Content <br/>
`subKey`: You need to use the **\_title** Property in **lowercase** like in Fortnite the 'shopSections' object has the '\_title' value of 'shop-sections' so use that as the subKey instead of 'shopSections'

## Query Parameters

`lang` - language of the response (e.g. 'en')

---

_Example Response (uefn - 'main-info', shortened)_

```json
{
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
  "_templateName": "FortniteEditorMain",
  "_suggestedPrefetch": []
}
```
