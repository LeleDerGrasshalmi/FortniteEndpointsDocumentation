## Global Service - Profile: Get Profiles

URL: https://global-profile-service.game-social.epicgames.com/profiles \
Method: PUT \
Auth Required: Yes (No Perm required)

```json
{
  "namespace": "",
  "accountIds": []
}
```

## Parameters

`namespace`: e.g. `Fortnite` \
`accountIds`: the account ids (up to 100)

---

_Example Response_

```json
{
  "profiles": [
    {
      "accountId": "94b1569506b04f9f8557af611e8c5e47",
      "hasBattlePass": false,
      "playRegion": "EUROPE",
      "hasCrewMembership": false,
      "languages": ["en"],
      "seasonLevel": 10
    }
  ]
}
```
