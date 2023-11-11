## FN - Discovery Service: Unlock Link

URL: https://fn-service-discovery-live-public.ogs.live.on.epicgames.com/api/v1/links/unlock/:accountId/:linkCode \
Method: PUT \
Auth Required: Yes (`discovery:{accountId}:links:lock-management UPDATE`)

## Path Parameters

`accountId`: Your Account Id <br/>
`linkCode`: The Mnemonic to unlock, e.g. `6276-3568-1807`

---

_Example Response (No IARC data set)_

```json
{
  "errorCode": "errors.com.epicgames.missing_player_ratings_body_setting",
  "errorMessage": "Missing player ratings authority setting for player id 94b1569506b04f9f8557af611e8c5e47"
}
```
