## Fortnite Website - Video Clips

URL: https://fortnite.com/:language/api/video-clips <br/>
Method: GET <br/>
Auth Required: Yes

## Path Parameters

`language`: The language or locale code.

---

*Example Response*

```json
{
  "success": true,
  "data": {
    "eligible": false,
    "ineligibleImage": "https://cdn2.unrealengine.com/Fortnite%2Fcustom-video-recap%2FsampleBg-3840x2160-ddb4aa89efe60de4b7925806e9736fbb61807809.png"
  }
}
```

<br/>

## Fortnite Website - Video Clips Post

URL: https://fortnite.com/:language/api/video-clips <br/>
Method: POST <br/>
Auth Required: Yes

```json
[
  {
    "key": "scene24",
    "val": "yes"
  },
  {
    "key": "user_color",
    "val": "blue"
  },
  {
    "key": "user_soundtrack",
    "val": "BunkerJam"
  }
]
```

The values can be gotten from the get request if you're eligible

## Path Parameters

`language`: The language or locale code.

---

*Example Response*

No example response or status is documented.
