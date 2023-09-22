## Account Web - History

URL: https://www.epicgames.com/account/v2/eula/acceptance-history \
Method: GET \
Auth Required: Yes

_Example Response_

```json
{
  "success": true,
  "message": "",
  "data": [
    {
      "key": "sac_agreement",
      "title": "SUPPORT-A-CREATOR PROGRAM TERMS",
      "locale": "en-US",
      "version": 2,
      "revision": 2,
      "accountId": "####",
      "identityId": "####",
      "accepted": true,
      "responseTimestamp": "2023-09-15T19:03:22.942Z",
      "url": "https://cdn1.epicgames.com/eulatracking-download/sac_agreement/en/v2/r2/b45bd70aa03b32a8cfb133413722c400.pdf"
    },
    {
      "key": "fn",
      "title": "Fortnite® End User License Agreement",
      "locale": "en-US",
      "version": 5,
      "revision": 8,
      "accountId": "####",
      "identityId": "####",
      "accepted": true,
      "responseTimestamp": "2022-03-24T12:01:28.943Z",
      "url": "https://cdn1.epicgames.com/eulatracking-download/fn/en/v5/r8/d3b60a9267a0b424d5c92f258e80814a.pdf"
    }
  ]
}
```