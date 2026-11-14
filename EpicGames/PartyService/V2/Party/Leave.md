## Party Service V2 - Leave / Kick

URL: https://api.epicgames.dev/epic/party/internal/v2/parties/:partyId/members/:accountId \
Method: DELETE \
Auth Required: Yes (Account Auth)

## Path Parameters

`partyId`: The Party ID <br/>
`accountId`: Your AccountId to leave, or another member's AccountId to kick (party lead only)

---

_Example Response_: Status 204

_Example Response (Party not found)_

```json
{
  "errorCode": "errors.com.epicgames.social.party.party_not_found",
  "errorMessage": "Party [2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f] does not exist.",
  "messageVars": [
    "2f1f0a5e3c8b4b6f9d7e1a2b3c4d5e6f"
  ],
  "numericErrorCode": 51002,
  "originatingService": "party-v2",
  "intent": "prod"
}
```
