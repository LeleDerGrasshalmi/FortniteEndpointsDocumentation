## Party Service - Join

URL: https://party-service-prod.ol.epicgames.com/party/api/v1/Fortnite/parties/:partyId/members/:accountId/join \
Method: POST \
Auth Required: Yes (`social:party`)

```json
    {
        "connection": {
            "id": "b1c60df4f45a4b51b763eac539326664@prod.ol.epicgames.com/V2:Fortnite:WIN::29526DE64917CE4A791736BEB2C78A46",
            "meta": {
                "urn:epic:conn:platform_s": "WIN",
                "urn:epic:conn:type_s": "game"
            },
            "yield_leadership": false
        },
        "meta": {
            "urn:epic:member:dn_s": "Entrapta",
            "urn:epic:member:joinrequestusers_j": "{\"users\":[{\"id\":\"b1c60df4f45a4b51b763eac539326664\",\"dn\":\"Entrapta\",\"plat\":\"WIN\",\"data\":{\"CrossplayPreference\":\"1\",\"SubGame_u\":\"1\"}}]}"
        }
    }
```


## Path Parameters

`partyId`: The current Party ID <br/>
`accountId`: Your AccountId

## Parameters
`id`: Your Fortnite XMPP JID <br/>
`urn:epic:conn:platform_s`: The current platform you're playing on <br/>
`urn:epic:conn:type_s`: Not quite sure what values this has but game is used when inviting people <br/>
`yield_leadership`: Always false when joining parties <br/>
`urn:epic:member:dn_s`: Your Epic Display Name <br/>
`urn:epic:member:joinrequestusers_j`: An stringified users array with your Epic ID, Display Name, Platform, & Cross-Play Settings

_Example Response_

```json
{
	"status": "JOINED",
	"party_id": "6d3d5a885262440d8ea0a2d91ce438c5"
}
```

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