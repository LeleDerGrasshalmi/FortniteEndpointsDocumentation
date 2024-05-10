## Friends Service - Update Privacy Settings

URL: https://friends-public-service-prod.ol.epicgames.com/friends/api/v1/:accountId/settings \
Method: PATCH \
Auth Required: Yes (`friends:{accountId} UPDATE`)

```json
{
  "acceptInvites": "public",
  "mutualPrivacy": "ALL"
}
```

## Path Parameters

`accountId`: Your Account Id

## Parameters

`acceptInvites`: Friend Request Privacy: PUBLIC, FRIENDS_OF_FRIENDS, PRIVATE (case insensitive, epic lowercases it) <br/>
`mutualPrivacy`: Mutual Privacy to Friends: ALL, FRIENDS, NONE

---

_Example Response_

```json
{
  "acceptInvites": "private",
  "mutualPrivacy": "ALL"
}
```

> **Historic Note** <br/>
> The Method originally was `PUT` but is `PATCH` now, `PUT` is a relict, it only updates the `acceptInvites` setting. <br/>
> Even if both settings are required in the body, likely caused by the fact, that they share the same request payload model.
