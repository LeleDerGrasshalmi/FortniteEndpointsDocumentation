## Account Web - Connections: Social Connections

URL: https://www.epicgames.com/account/v2/connections/socialConnection/ajaxGet \
Method: GET \
Auth Required: Yes

## Query Parameters

`lang`: Specify the Link Language

---

_Example Response_

```json
{
  "socialData": {
    "githubDisplayName": "LeleDerGrasshalmi",
    "githubConnected": false,
    "twitchDisplayName": "Fortnite",
    "twitchConnected": false,
    "twitchLinkUrl": "https://www.epicgames.com/id/link/twitch?productName=fortnite&successRedirect=https%3A%2F%2Fwww.epicgames.com%2Faccount%2Fconnections%3Flang%3Den-US%23accounts&client_id=007c0bfe154c4f5396648f013c641dcf&lang=en_US",
    "psnLinkUrl": "https://www.epicgames.com/id/link/psn?productName=fortnite&successRedirect=https%3A%2F%2Fwww.epicgames.com%2Faccount%2Fconnections%3Flang%3Den-US%23accounts&client_id=007c0bfe154c4f5396648f013c641dcf&lang=en_US",
    "xboxLinkUrl": "https://www.epicgames.com/id/link/xbl?productName=fortnite&successRedirect=https%3A%2F%2Fwww.epicgames.com%2Faccount%2Fconnections%3Flang%3Den-US%23accounts&client_id=007c0bfe154c4f5396648f013c641dcf&lang=en_US",
    "nintendoLinkUrl": "https://www.epicgames.com/id/link/nintendo?productName=fortnite&successRedirect=https%3A%2F%2Fwww.epicgames.com%2Faccount%2Fconnections%3Flang%3Den-US%23accounts&client_id=007c0bfe154c4f5396648f013c641dcf&lang=en_US",
    "legoLinkUrl": "https://www.epicgames.com/id/link/lego?productName=fortnite&successRedirect=https%3A%2F%2Fwww.epicgames.com%2Faccount%2Fconnections%3Flang%3Den-US%23accounts&client_id=007c0bfe154c4f5396648f013c641dcf&lang=en_US",
    "githubLinkUrl": "https://www.epicgames.com/id/link/github?productName=fortnite&successRedirect=https%3A%2F%2Fwww.epicgames.com%2Faccount%2Fconnections%3Flang%3Den-US%23accounts&client_id=007c0bfe154c4f5396648f013c641dcf&lang=en_US",
    "steamLinkUrl": "https://www.epicgames.com/id/link/steam?productName=fortnite&successRedirect=https%3A%2F%2Fwww.epicgames.com%2Faccount%2Fconnections%3Flang%3Den-US%23accounts&client_id=007c0bfe154c4f5396648f013c641dcf&lang=en_US"
  },
  "externalAuths": [
    {
      "accountId": "94b1569506b04f9f8557af611e8c5e47",
      "type": "google",
      "externalAuthId": "0",
      "externalAuthIdType": "google_user_id",
      "externalDisplayName": "Lele",
      "authIds": [
        {
          "id": "0",
          "type": "google_user_id"
        }
      ],
      "dateAdded": "2023-08-21T17:09:00.824Z",
      "connected": false
    },
    {
      "accountId": "",
      "type": "steam",
      "externalAuthId": "",
      "externalDisplayName": "",
      "externalAuthIdType": "",
      "authIds": [],
      "dateAdded": "",
      "connected": false,
      "linkUrl": "https://www.epicgames.com/id/link/steam?productName=fortnite&successRedirect=https%3A%2F%2Fwww.epicgames.com%2Faccount%2Fconnections%3Flang%3Den-US%23accounts&client_id=007c0bfe154c4f5396648f013c641dcf&lang=en_US"
    }
  ],
  "featuredApps": []
}
```
