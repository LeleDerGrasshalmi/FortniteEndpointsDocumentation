## Library Service - Artifact Playtime

URL: https://library-service.live.use1a.on.epicgames.com/library/api/public/playtime/account/:accountId/artifact/:artifactId \
Method: GET \
Auth Required: Yes (`library:public:{accountId}:playtime READ`)

## Path Parameters

`accountId`: Your Account Id <br/>
`artifactId`: The Artifact Id, e.g. `Fortnite` for Fortnite (See [How to obtain it](../../README.md#obtaining-the-artifact-id))

---

_Example Response_

```json
{
  "accountId": "94b1569506b04f9f8557af611e8c5e47",
  "artifactId": "Fortnite",
  "totalTime": 86164
}
```
