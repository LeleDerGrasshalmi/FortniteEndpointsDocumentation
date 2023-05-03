## Fortnite - Content

URL: https://fortnitecontent-website-prod07.ol.epicgames.com/content/api/pages/fortnite-game \
Method: GET \
Auth Required: No

### Query

`lang` - language of the response (e.g. 'en')

> Specific Data Only: <br/>
> You need to use the **\_title** Property in **lowercase** like `https://fortnitecontent-website-prod07.ol.epicgames.com/content/api/pages/fortnite-game/:_title` <br/>
> For Example we take the 'shopSections' Data, when requesting `https://fortnitecontent-website-prod07.ol.epicgames.com/content/api/pages/fortnite-game/shopSections` <br/>
> we will get status 404, but when using the `'_title' property` which is 'shop-sections' we get status 200
