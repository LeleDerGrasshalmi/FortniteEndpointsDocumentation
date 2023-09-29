## Fortnite Website - POSA: Content

URL: https://fortnite.com/:locale/api/posa/content \
Method: GET \
Auth Required: No

## Path Parameters

`locale`: The Locale of the Response, defaults to `en-US` if invalid

---

_Example Response (Shortened)_

```json
{
  "success": true,
  "page": {
    "configs": {
      "enableRegionAutoDetection": true,
      "enablePOSA": true,
      "extra": "*This device doesn't appear to be linked to this account. Please check that you entered the correct account.",
      "_type": "POSA Redemption Configs",
      "id": "fortnite-posa-redemption",
      "psnOptions": "[\n    {\n        \"label\": \"United States\",\n        \"value\": \"us\"\n    },\n{\n\"label\": \"Germany\",\n\"value\": \"de\"\n},\n{\n\"label\": \"France\",\n\"value\": \"fr\"\n},\n{\n\"label\": \"United Kingdom\",\n\"value\": \"gb\"\n},\n    {\n        \"label\": \"Chile\",\n        \"value\": \"cl\"\n    },\n    {\n        \"label\": \"Honduras\",\n        \"value\": \"hn\"\n    },\n    {\n        \"label\": \"Canada\",\n        \"value\": \"ca\"\n    },\n    {\n        \"label\": \"Colombia\",\n        \"value\": \"co\"\n    },\n    {\n        \"label\": \"Nicaragua\",\n        \"value\": \"ni\"\n    },\n    {\n        \"label\": \"Mexico\",\n        \"value\": \"mx\"\n    },\n    {\n        \"label\": \"Costa Rica\",\n        \"value\": \"cr\"\n    },\n    {\n        \"label\": \"Panama\",\n        \"value\": \"pa\"\n    },\n    {\n        \"label\": \"Brazil\",\n        \"value\": \"br\"\n    },\n    {\n        \"label\": \"Ecuador\",\n        \"value\": \"ec\"\n    },\n    {\n        \"label\": \"Paraguay\",\n        \"value\": \"py\"\n    },\n    {\n        \"label\": \"Argentina\",\n        \"value\": \"ar\"\n    },\n    {\n        \"label\": \"El Salvador\",\n        \"value\": \"sv\"\n    },\n    {\n        \"label\": \"Peru\",\n        \"value\": \"pe\"\n    },\n    {\n        \"label\": \"Bolivia\",\n        \"value\": \"bo\"\n    },\n    {\n        \"label\": \"Guatemala\",\n        \"value\": \"gt\"\n    },\n    {\n        \"label\": \"Uruguay\",\n        \"value\": \"uy\"\n    },\n    {\n        \"label\" : \"Spain\",\n        \"value\" : \"es\"\n    },\n    {\n        \"label\": \"Portugal\",\n        \"value\": \"pt\"\n    },\n    {\n        \"label\": \"Italy\",\n        \"value\": \"it\"\n    },\n    {\n        \"label\": \"Japan\",\n        \"value\": \"JAPAN\"\n    },\n    {\n        \"label\":\"More Countries Coming Soon\",\n        \"value\":\"xxx\",\n        \"disabled\":true\n    }\n]"
    },
    "_title": "POSA Card Redemption",
    "_noIndex": false,
    "xblSuccess": {
      "visitText": "GO TO MICROSOFT.COM",
      "visitLink": "https://microsoft.com/redeem",
      "_type": "POSA Success Content",
      "contentRightColumn": "<h3>XBOX CODE</h3>\n\n<h1>{secondaryCode}</h1>\n\n<h3>THEN DO THE FOLLOWING:</h3>\n\n<ul>\n    <li><span class=\"circle\">1</span>\n\n    <h4>VISIT <a href=\"https://microsoft.com/redeem\" target=\"_blank\">MICROSOFT.COM/REDEEM</a> AND SIGN IN WITH YOUR MICROSOFT CREDENTIALS</h4>\n    </li>\n    <li><span class=\"circle\">2</span>\n    <div>\n    <h4>CLICK YOUR USERNAME IN THE TOP RIGHT, THEN ‘REDEEM CODES’</h4>\n\n    <p>For more details see the carousel of images below to help you redeem your Xbox code. Your Xbox code is always accessible here, just re-enter your V-Bucks Card code on this site to find it again. Keep your V-Bucks Card safe until the V-Bucks are in your wallet in Fortnite.</p>\n    </div>\n    </li>\n    <li class=\"copyToClipboard\"> </li>\n    <li class=\"visitLink\"> </li>\n</ul>\n",
      "bgImage": "https://cdn2.unrealengine.com/Fortnite%2Fposa-card-redemption%2FBG_1907x939_1567968566929_1907x878_1569312335335-1907x877-d35d9e0920677225dd2b1065a0193fa848712bfa.png",
      "disableStepsButton": false,
      "contentLeftColumn": "<h1>ALMOST DONE...</h1>\n\n<h3>TO GET YOUR {cardBalance} V-BUCKS INTO YOUR WALLET, YOU NEED TO DO A FEW THINGS. FIRST, WRITE DOWN THIS XBOX CODE</h3>\n",
      "sliderSection": {
        "slide": [
          {
            "image": "https://cdn2.unrealengine.com/Fortnite%2Fposa-card-redemption%2FxboxScreen-830x467-51ece10577f9b4df4e0e534d7efb56e812a4763e.png",
            "_type": "POSA Success Slider Item",
            "tips": "<p>Having trouble? Write down your Xbox code above and reach out to Fortnite’s <a href=\"https://com/support?contact=1\" target=\"_blank\">customer support team</a> for help.</p>\n"
          }
        ],
        "_type": "POSA Success Slider Section",
        "title": "WHERE TO ENTER THE CODE ON YOUR XBOX"
      }
    },
    "_images_": [
      "https://cdn2.unrealengine.com/1920x1080-1920x1080-917435454.png"
    ],
    "sections": {
      "_type": "POSA Sections",
      "sections": [
        {
          "_type": "POSA",
          "redeemSection": {
            "moneyImage": "https://cdn2.unrealengine.com/faq-singular-card-102721-739x1023-651e0791cffe.png",
            "toolTipDescription": "<h1>WHERE DO I FIND THIS?</h1>\n\n<p>The code (PIN) you need is located on the back of the card under a scratch off security covering.</p>\n\n<p><em>Disclaimer: Please note that the PIN on the back of your card can only be redeemed through this website.</em></p>\n",
            "unLoggedInContent": "<h1>REDEEM YOUR <span style=\"white-space:nowrap\">V-BUCKS</span> CARD</h1>\n\n<h2>\n<style type=\"text/css\"><!--td {border: 1px solid #ccc;}br {mso-data-placement:same-cell;}-->\n</style>\nCARDS PURCHASED AT RETAIL STORES ARE REDEEMED HERE</h2>\n\n<p>An Epic Games account is required to redeem a V-Bucks Card code. If you have played Fortnite, you already have an Epic Games account. Click <strong>Get Started</strong> below to find your Epic Games account and redeem your V-Bucks!</p>\n",
            "_type": "POSA Redeem Section",
            "platformToolTip": "<h1>Why do I have to choose a platform?</h1>\n\n<p>Choose the game device or console platform where you want to spend your V-Bucks. Redemption is only allowed on game devices you’ve already played Fortnite on. Nintendo Switch V-Bucks can only be spent on that platform. On all other platforms, your V-Bucks wallet is shared (see <a href=\"http://fn.gg/vbucks\" target=\"_blank\">fn.gg/vbucks</a> for more information).</p>\n",
            "loggedInContent": "<h1>Alright {epicAccountName}, <span class=\"nobreak\">Let’s Do This!</span></h1>\n\n<h2>Turn over your card and scratch off the security covering.</h2>\n\n<p>Since you're logged into your Epic account, please enter the code from the back of your V-Bucks card below. Then choose the device you play Fortnite on.</p>\n",
            "bgImage": "https://cdn2.unrealengine.com/Fortnite%2Fposa-card-redemption%2FBG_1907x939_1567968566929_1907x878_1569312335335-1907x877-d35d9e0920677225dd2b1065a0193fa848712bfa.png",
            "psnToolTip": "<h1>Why do I have to choose a region?</h1>\n\n<p>There is no current way for players to determine their PlayStation account region. We have selected the most likely region based on where you play Fortnite. If you are certain that your region is different than our selection, you may change it.</p>\n\n<p><em>If you select the incorrect PlayStation region for your account it will be impossible for you to redeem your V-Bucks. Please contact Sony Customer support if you are concerned: <a href=\"https://support.playstation.com\" target=\"_blank\">https://support.playstation.com</a> </em></p>\n",
            "toolTipImage": "https://cdn2.unrealengine.com/Fortnite%2Fposa-card-redemption%2FLayer-1_1515x1331_1568656048390-1515x1331-3072bcfd91da7c00d17ae0411cfbd0944e1d2515.png"
          }
        },
        {
          "_type": "POSA",
          "richText": {
            "_type": "POSA Rich Text",
            "content": "<p>Redeem a gift card for V-Bucks to use in Fortnite on any supported device! To use a gift card you must have a valid Epic Account, download Fortnite on a compatible device, and accept the applicable terms and user agreement. Review your device maker’s terms for any additional requirements to play Fortnite (e.g., subscriptions, additional fees). Visit <a href=\"/vbuckscardterms\" target=\"_blank\">fortnite.com/vbuckscardterms</a> to read the full terms before purchasing. The card’s full face-value is deducted at redemption and associated with a single account for the device you select (no transfer or withdrawal). A gift card can only be redeemed for the indicated amount of V-Bucks, which may only be used in Fortnite. There are no fees or expiration dates associated with the use of a gift card. V-Bucks aren’t e-money or any other currency and can only be used according to Fortnite’s rules. Gift cards will not be replaced if lost, stolen, destroyed, or used without permission. Use of a gift card constitutes acceptance of the applicable terms and user agreement.<br />\n<br />\n©2023, Epic Games, Inc., Epic Games®, Fortnite®, their logos, and V-Bucks are trademarks of Epic Games, Inc. PlayStation®4, PlayStation®5, Xbox One™, Xbox Series X™, Xbox Series S™, Nintendo Switch™, PC, Android™, and the ratings icon are the trademarks of their respective owners. Gift cards are issued and distributed by Epic Games Inc., Epic Games Entertainment International GmbH. For support visit fortnite.com/support.</p>\n"
          }
        },
        {
          "ctaSection": {
            "cta": {
              "textOne": "JUMP IN",
              "_type": "CTA Link"
            },
            "rightContent": "<h1>GET THE NEW BATTLE PASS</h1>\n\n<h3>ONLY 950 V-BUCKS</h3>\n\n<p>The more you play, the more rewards you unlock. Earn XP to unlock exclusive rewards like Outfits, Emotes, Back Blings, Wraps, Pets, and more!</p>\n",
            "_type": "POSA CTA Section",
            "bgImage": "https://cdn2.unrealengine.com/Fortnite%2Fposa-card-redemption%2FRectangle-9-1924x761-584649107dc5a0508e9c17fef4d5f433c71d729d.png",
            "leftImage": "https://cdn2.unrealengine.com/Fortnite%2Fposa-card-redemption%2FGroup-1_1105x996_1568652773811_1099x995_1568652787381-1098x995-90179540f97032b15abfcb6766ae48db48b10750.png"
          },
          "_type": "POSA"
        },
        {
          "faqSection": {
            "image": "https://cdn2.unrealengine.com/faq-angled-cards-102721-759x793-91fa5b26d6ca.png",
            "subTitle": "V-BUCKS CARDS ARE AVAILABLE AT MAJOR RETAILERS IN THE USA, CANADA, AUSTRALIA, AUSTRIA, BELGIUM, FRANCE, GERMANY, IRELAND, ITALY, JAPAN, THE NETHERLANDS, NEW ZEALAND, PORTUGAL, SPAIN AND UNITED KINGDOM ",
            "_type": "POSA FAQ Section",
            "faqList": [
              {
                "question": "What are V-Bucks?",
                "answer": "V-Bucks are an in-game currency used in Fortnite.",
                "_type": "POSA FAQ Item"
              }
            ],
            "title": "V-BUCKS CARD FAQs"
          },
          "_type": "POSA"
        }
      ]
    },
    "loginModal": {
      "warningContent": "<h1>HAVEN&#39;T PLAYED BEFORE?</h1>\n\n<p>V-Bucks cards should only be redeemed on the account where they will be spent.</p>\n\n<p>To make sure your V-Bucks are available on the platform where you will play, please install and launch Fortnite on your chosen game device.</p>\n\n<p>Then come back to the site, and follow the instructions to finish redeeming your V-Bucks card.</p>\n",
      "_type": "POSA Login Modal"
    },
    "_metaTags": "<!-- Open Graph data for Facebook -->\n<meta property=\"og:type\" content=\"article\">\n<meta property=\"og:title\" content=\"Learn About Fortnite V-Bucks and How to Redeem V-Bucks Gift Cards\">\n<meta property=\"og:description\" content=\"Fortnite V-Bucks is our in-game currency used to purchase items. Also, learn how to redeem your V-Bucks Gift Cards sold at retail stores.\">\n<meta property=\"og:image\" content=\"https://cdn2.unrealengine.com/Fortnite%2Fposa-card-redemption%2FAngledCardImages_cropped-1920x1080-5553b39dff9d579d9cbbb48d5600b53861d3ff87.jpg\">\n<meta property=\"og:url\" content=\"https://www.epicgames.com/fortnite/\">\n\n<!-- Twitter Card data -->\n<meta name=\"twitter:card\" content=\"summary\">\n<meta name=\"twitter:title\" content=\"Learn About Fortnite V-Bucks and How to Redeem V-Bucks Gift Cards\">\n<meta name=\"twitter:description\" content=\"Fortnite V-Bucks is our in-game currency used to purchase items. Also, learn how to redeem your V-Bucks Gift Cards sold at retail stores.\">\n<meta name=\"twitter:image\" content=\"https://cdn2.unrealengine.com/Fortnite%2Fposa-card-redemption%2FAngledCardImages_cropped-1920x1080-5553b39dff9d579d9cbbb48d5600b53861d3ff87.jpg\">",
    "psnSuccess": {
      "visitText": "VISIT PLAYSTATION NETWORK",
      "visitLink": "https://store.playstation.com",
      "_type": "POSA Success Content",
      "contentRightColumn": "<h3>PLAYSTATION CODE</h3>\n\n<h1>{secondaryCode}</h1>\n\n<h3>THEN DO THE FOLLOWING:</h3>\n\n<ul>\n    <li><span class=\"circle\">1</span>\n\n    <h4>TURN ON YOUR PLAYSTATION AND NAVIGATE TO THE PLAYSTATION STORE.</h4>\n    </li>\n    <li><span class=\"circle\">2</span>\n    <h4>CHOOSE 'REDEEM CODE'</h4>\n    </li>\n    <li><span class=\"circle\">3</span>\n    <h4>ENTER THIS CODE ABOVE INTO THE FIELD ON YOUR PLAYSTATION</h4>\n    </li>\n    <li><span class=\"circle\">4</span>\n    <h4>CLICK “REDEEM” AND CONFIRM YOUR PURCHASE TO RECEIVE YOUR V-BUCKS</h4>\n    </li>\n</ul>\n\n<p>See the image below. Alternatively, you can redeem your code online through your computer or phone at <a href=\"https://store.playstation.com\" target=\"_blank\">https://store.playstation.com</a></p>\n\n<p>Your PlayStation code is always accessible under your transaction history page on your account management page. It was also emailed to your Epic Games account's email address. Keep your V-Bucks card safe until the V-Bucks are in your wallet in Fortnite, as it might be needed if you require Player Support!</p>\n",
      "bgImage": "https://cdn2.unrealengine.com/Fortnite%2Fposa-card-redemption%2FBG_1907x939_1567968566929_1907x878_1569312335335-1907x877-d35d9e0920677225dd2b1065a0193fa848712bfa.png",
      "disableStepsButton": true,
      "contentLeftColumn": "<h1>ALMOST DONE...</h1>\n\n<h3>TO GET YOUR {cardBalance} V-BUCKS INTO YOUR WALLET, YOU NEED TO DO A FEW THINGS. FIRST, WRITE DOWN THIS PLAYSTATION {psnRegionName} CODE</h3>\n",
      "sliderSection": {
        "slide": [
          {
            "image": "https://cdn2.unrealengine.com/Fortnite%2Fposa-card-redemption%2FpsnScreen-1600x900-76b7a920ef5cb4113364267cdfd34e4d177d930b.png",
            "_type": "POSA Success Slider Item",
            "tips": "<p>Having trouble? Write down your PlayStation code above and reach out to Fortnite’s <a href=\"https://com/support?contact=1\" target=\"_blank\">customer support team</a> for help.</p>\n"
          }
        ],
        "subtitle": "",
        "_type": "POSA Success Slider Section",
        "title": "WHERE TO ENTER THE CODE ON YOUR PLAYSTATION"
      }
    },
    "generalSuccess": {
      "_type": "POSA Success Content",
      "contentRightColumn": "<h1>YOU HAVE <span class=\"nobreak\">V-BUCKS!</span></h1>\n\n<h3 style=\"color: #ff0\">YOU’VE REDEEMED <span class=\"nobreak\" style=\"color: white\">{cardBalance} V-BUCKS</span>, AND WE’VE ADDED IT TO YOUR IN-GAME WALLET. DROP IN TO FORTNITE TO SPEND YOUR <span class=\"nobreak\">V-BUCKS.</span></h3>\n\n<div class=\"centered\"><a class=\"btn btn-primary centered restart\">Redeem Another Card</a></div>\n",
      "bgImage": "https://cdn2.unrealengine.com/Fortnite%2Fposa-card-redemption%2FBG_1907x939_1567968566929_1907x878_1569312335335-1907x877-d35d9e0920677225dd2b1065a0193fa848712bfa.png",
      "disableStepsButton": true,
      "contentLeftColumn": "<img src=\"{cardImage}\" />\n",
      "sliderSection": {
        "_type": "POSA Success Slider Section"
      }
    },
    "metaTags": {
      "image": "https://cdn2.unrealengine.com/1920x1080-1920x1080-917435454.png",
      "keyWords": "",
      "_type": "Epic Common Share Meta Data",
      "description": "Fortnite V-Bucks is our in-game currency used to purchase items. Also, learn how to redeem your V-Bucks Gift Cards sold at retail stores.",
      "title": "Fortnite V-Bucks | Redeem V-Bucks Gift Card - Fortnite"
    },
    "messages": "{\n}",
    "_urlPattern": "/posa-card-redemption",
    "_slug": "posa-card-redemption",
    "_activeDate": "2023-07-03T01:00:00.000Z",
    "lastModified": "2023-07-31T14:24:54.320Z",
    "_locale": "en-US",
    "_id": "426416d5-b13c-42c6-a523-cd5f96a41285",
    "_templateName": "posaCard"
  }
}
```
