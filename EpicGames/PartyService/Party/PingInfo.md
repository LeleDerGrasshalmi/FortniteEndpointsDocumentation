## Party Service - Get Party Info by Party Invite Ping

URL: https://party-service-prod.ol.epicgames.com/party/api/v1/Fortnite/user/:accountId/pings/:pingerId/parties \
Method: GET \
Auth Required: Yes (`social:party`)

## Path Parameters

`accountId`: Your AccountId <br/>
`pingerId`: AccountId of who invited you

_Example Response (shortened)_

```json
[
	{
		"id": "da867bd83ebe4035ac874676c647bcb3",
		"created_at": "2025-09-01T00:57:39.320Z",
		"updated_at": "2025-09-01T00:57:39.907Z",
		"config": {
			"type": "DEFAULT",
			"joinability": "INVITE_AND_FORMER",
			"discoverability": "INVITED_ONLY",
			"sub_type": "default",
			"max_size": 16,
			"invite_ttl": 14400,
			"join_confirmation": true,
			"intention_ttl": 7200
		},
		"members": [],
		"applicants": [],
		"meta": {
			"Default:PartyState_s": "BattleRoyaleView",
			"urn:epic:cfg:build-id_s": "1:3:45178693",
			"Default:RegionId_s": "NAE",
			"Default:PrivacySettings_j": "{\"PrivacySettings\":{\"partyType\":\"Private\",\"partyInviteRestriction\":\"AnyMember\",\"bOnlyLeaderFriendsCanJoin\":false}}",
			"Default:GameSessionKey_s": "",
			"urn:epic:cfg:chat-enabled_b": "true",
			"Default:PartyMatchmakingInfo_j": "{\"PartyMatchmakingInfo\":{\"buildId\":-1,\"hotfixVersion\":-1,\"regionId\":\"\",\"playlistName\":\"None\",\"playlistRevision\":0,\"tournamentId\":\"\",\"eventWindowId\":\"\",\"linkCode\":\"\"}}",
			"urn:epic:cfg:can-join_b": "true"
		},
		"invites": [
			{
				"party_id": "da867bd83ebe4035ac874676c647bcb3",
				"sent_by": "b1c60df4f45a4b51b763eac539326664",
				"meta": {
					"urn:epic:conn:platform_s": "WIN",
					"urn:epic:member:dn_s": "Entrapta",
					"urn:epic:cfg:build-id_s": "1:3:44594305",
					"urn:epic:invite:platformdata_s": "guid=435B10344BD59D9426996BAE682B5015"
				},
				"sent_to": "b006e6841d30478db7fcc1151b476d1c",
				"sent_at": "2025-09-01T00:58:04.639Z",
				"updated_at": "2025-09-01T00:58:04.639Z",
				"expires_at": "2025-09-01T04:58:04.639Z",
				"status": "SENT"
			}
		],
		"revision": 1,
		"intentions": []
	}
]
```