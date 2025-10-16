## Party Service - Update Party Metadata

URL: https://party-service-prod.ol.epicgames.com/party/api/v1/Fortnite/parties/:partyId
Method: PATCH \
Auth Required: Yes (`social:party`)

```json
{
  "revision": 3,
  "meta": {
    "update": {
      "Default:SquadInformation_j": "{\"SquadInformation\":{\"rawSquadAssignments\":[{\"memberId\":\"b1c60df4f45a4b51b763eac539326664\",\"absoluteMemberIdx\":-100}]"
    }
  }
}

```

## Path Parameters

`partyId`: Party Id

## Parameters

`revision`: An number that increments with every party meta change. <br/>
`meta.update`: An object with the specific key you want updated. (Some values might be required to be stringified)

_Example Reponse_: Status 204

_Example Response (Incorrect revision number)_

```json
{
	"errorCode": "errors.com.epicgames.social.party.stale_revision",
	"errorMessage": "Provided revision [2] does not match the current one [1].",
	"numericErrorCode": 51018,
	"originatingService": "party",
	"intent": "prod"
}
```