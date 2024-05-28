## EGS Platform Service - Product Info

URL: https://egs-platform-service.store.epicgames.com/api/v1/egs/products/:productId \
Method: GET \
Auth Required: No

## Query Parameters

`country`: (required) ISO 3166 - Alpha 2 Code <br/>
`locale`: (required) e.g. 'de' (German), fallback is 'en' <br/>
`store`: (required) valid Catalog Service Stores, e.g. `EGS`

## Path Parameters

`productId`: self explaining, e.g. `prod-fn` for Fortnite

---

_Example Response_

```json
{
  "__typename": "Product",
  "branding": {
    "dark": {
      "accentColor": "#F5CA23",
      "brandColor": "gray"
    },
    "light": {
      "accentColor": "#F5CA23",
      "brandColor": "gray"
    },
    "preferredMode": "dark"
  },
  "developers": ["Epic Games"],
  "id": "prod-fn",
  "mapping": {
    "__typename": "InternalMapping",
    "slug": "fortnite"
  },
  "media": {
    "card16x9": {
      "imageSrc": "https://cdn1.epicgames.com/offer/fn/Blade_2560x1440_2560x1440-95718a8046a942675a0bc4d27560e2bb"
    },
    "card3x4": {
      "imageSrc": "https://cdn1.epicgames.com/offer/fn/Blade_1200x1600_1200x1600-fcea56f5eb92df731a89121e2b4416b5"
    },
    "logo": {
      "altText": "Fortnite Logo",
      "imageSrc": "https://cdn2.unrealengine.com/24br-s24-egs-launcher-logo-350x100-350x100-b63249f937d9.png"
    }
  },
  "publishers": ["Epic Games"],
  "shortDescription": "Create, play, and battle with friends for free in Fortnite. Be the last player standing in Battle Royale and Zero Build, experience a concert or live event, or discover over a million creator made games, including racing, parkour, zombie survival, and more.  Each Fortnite island has an individual age rating so you can find the one that's right for you and your friends. Find it all in Fortnite ... Drop In.",
  "supportedModules": {
    "addOns": true,
    "criticReviews": {
      "openCritic": true
    },
    "editions": false,
    "experiences": true,
    "mods": "Unsupported"
  },
  "tags": {
    "accessibility": [],
    "epicFeatures": [],
    "events": [],
    "features": [
      {
        "id": "1264",
        "name": "Co-op"
      },
      {
        "id": "1299",
        "name": "Competitive"
      },
      {
        "id": "9549",
        "name": "Controller Support"
      },
      {
        "id": "1203",
        "name": "Multiplayer"
      },
      {
        "id": "1370",
        "name": "Single Player"
      }
    ],
    "genres": [
      {
        "id": "1216",
        "name": "Action"
      },
      {
        "id": "1210",
        "name": "Shooter"
      }
    ],
    "platforms": [
      {
        "id": "9547",
        "name": "Windows"
      }
    ],
    "usersSay": [
      {
        "id": "21139",
        "name": "Amazing Characters"
      },
      {
        "id": "21140",
        "name": "Amazing Storytelling"
      },
      {
        "id": "21125",
        "name": "Competitive Community"
      },
      {
        "id": "21122",
        "name": "Diverse Characters"
      },
      {
        "id": "21141",
        "name": "Extremely Fun"
      },
      {
        "id": "21149",
        "name": "Quickly Understand the Controls"
      },
      {
        "id": "21138",
        "name": "Recommend this Game"
      }
    ]
  },
  "title": "Fortnite"
}
```
