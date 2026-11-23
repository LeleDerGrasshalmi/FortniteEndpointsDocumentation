## Party Service - Promote

URL: https://party-service-prod.ol.epicgames.com/party/api/v1/Fortnite/parties/:partyId/members/:memberId/promote <br/>
Method: POST <br/>
Auth Required: Yes (`social:party`)

## Path Parameters

`partyId`: The current Party ID <br/>
`memberId`: Party member AccountId

---

*Example Response*: Status 204

*Example Response (User is not party leader)*

```json
{
  "errorCode": "errors.com.epicgames.social.party.party_change_forbidden",
  "errorMessage": "User [b1c60df4f45a4b51b763eac539326664] is not authorized to perform the action in party [18aabf9bcb4346a8b193d39d3f623e1e].",
  "numericErrorCode": 51015,
  "originatingService": "party",
  "intent": "prod"
}
```
