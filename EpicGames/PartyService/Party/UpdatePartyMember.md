## Party Service - Update Party Member Metadata

URL: https://party-service-prod.ol.epicgames.com/party/api/v1/Fortnite/parties/:partyId/members/:accountId/meta
Method: PATCH \
Auth Required: Yes (`social:party`)

```json
{
	"revision": 2,
	"update": {
		"Default:FrontendEmote_j": "{\"FrontendEmote\":{\"emoteItemDef\":\"/SparksSongTemplates/Items/JamEmotes/EID_Placeholder_35_Drum.EID_Placeholder_35_Drum\"}}"
	}
}
```

## Path Parameters

`partyId`: Party Id
`accountId`: Your AccountId

## Parameters

`revision`: An number that increments with every party meta change. <br/>
`update`: An object with the specific key you want updated. (Some values might be required to be stringified)

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