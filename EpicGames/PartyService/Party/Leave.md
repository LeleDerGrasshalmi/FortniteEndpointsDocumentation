## Party Service - Leave

URL: https://party-service-prod.ol.epicgames.com/party/api/v1/Fortnite/parties/:partyId/members/:accountId \
Method: DELETE \
Auth Required: Yes (`social:party`)

## Path Parameters

`partyId`: The current Party ID <br/>
`accountId`: Your AccountId

_Example Response_: Status 204

_Example Response (Party not found)_

```json
{
	"errorCode": "errors.com.epicgames.social.party.party_not_found",
	"errorMessage": "Party [226d9232419440f3a53578a3185f9933] does not exist.",
	"numericErrorCode": 51002,
	"originatingService": "party",
	"intent": "prod"
}
```