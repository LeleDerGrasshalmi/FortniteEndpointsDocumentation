## Party Service - Invite

URL: https://party-service-prod.ol.epicgames.com/party/api/v1/Fortnite/parties/:partyId/invites/:friendId?sendPing=true \
Method: POST \
Auth Required: Yes (`social:party`)

```json
{
    "urn:epic:cfg:build-id_s": "1:3:45178693",
    "urn:epic:conn:platform_s": "WIN",
    "urn:epic:conn:type_s": "game",
    "urn:epic:invite:platformdata_s": "",
    "urn:epic:member:dn_s": "Entrapta"
}
```

## Path Parameters

`partyId`: Your Party ID <br/>
`friendId`: Friend AccountId

## Parameters

`urn:epic:cfg:build-id_s`: Party Service Build ID <br/>
`urn:epic:conn:platform_s`: The current platform you're playing on ("XSX", "PS5", "AND", "IOS", "SWT", "XBL", "PSN", "MAC", "WIN") <br/>
`urn:epic:conn:type_s`: Not quite sure what values this has but game is used when inviting people <br/>
`urn:epic:invite:platformdata_s`: Always empty <br/>
`urn:epic:member:dn_s`: Your Epic Games Display Name

## Query Parameters

`sendPing`: If your party is invite only, set to true

_Example Response_: Status 204

_Example Response (Invite already sent)_

```json
{
	"errorCode": "errors.com.epicgames.social.party.invite_already_exists",
	"errorMessage": "Invite for user [b006e6841d30478db7fcc1151b476d1c] to party [bc70d384c4fa41249e77342cfbbab56b] already exists.",
	"numericErrorCode": 51009,
	"originatingService": "party",
	"intent": "prod"
}
```