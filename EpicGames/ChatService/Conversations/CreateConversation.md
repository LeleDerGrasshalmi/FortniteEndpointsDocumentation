## Chat Service - Conversations: Create Conversation

Creates a group conversation. Only the creator becomes a member, every other account in `members` is invited and joins with [Update Invite Status](./UpdateInviteStatus.md).

URL: https://api.epicgames.dev/epic/chat/v1/public/:namespace/conversations \
Method: POST \
Auth Required: Yes (Account Auth)

```json
{
  "title": "Docs Test",
  "members": ["c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60", "94b1569506b04f9f8557af611e8c5e47"],
  "type": "group"
}
```

## Path Parameters

`namespace`: e.g. `_`

## Parameters

`title`: Group title <br/>
`members`: AccountIds, must include your own AccountId <br/>
`type`: `group`

## Query Parameters

`invite`: `true`

---

_Example Response_

```json
{
  "conversationId": "07c0ExampleGroupId0001",
  "dateCreated": "2026-10-14T22:29:51.034Z",
  "isActive": true,
  "isReportable": false,
  "members": ["c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60"],
  "invited": ["94b1569506b04f9f8557af611e8c5e47"]
}
```

_Example Response (Same accounts as an existing group)_

If the accounts (members + invited) match an existing active group, that group is returned with `isExisting: true` and its original title is kept. Groups with 2 accounts (you + one invite) are accepted.

```json
{
  "conversationId": "07c0ExampleGroupId0005",
  "dateCreated": "2026-10-14T22:54:12.127Z",
  "isActive": true,
  "isReportable": true,
  "members": ["c1f0a37e2b6d4e8a9f5c7d1e3b2a4f60"],
  "invited": ["94b1569506b04f9f8557af611e8c5e47", "5e2d8c1b9a7f4e3d8c6b2a1f0e9d7c3b"],
  "isExisting": true
}
```

_Example Response (Own AccountId missing from `members`)_

```json
{
  "messageVars": [],
  "errorMessage": "Requesting account should be included in the members list",
  "errorCode": "errors.com.epicgames.bad_request",
  "correlationId": "5b8e2f1a-7c3d-4e6f-9a0b-1c2d3e4f5a6b",
  "numericErrorCode": 1001,
  "responseStatus": 400,
  "intent": "prod",
  "originatingService": "chat-service-api-prod"
}
```
