## Avatar Service - Avatar Assignments

Avatars of your friends, of the members of a party, or of the members of group chats.

URL (friends): https://api.epicgames.dev/epic/avatar/v1/:deploymentId/assignments/friends \
URL (party): https://api.epicgames.dev/epic/avatar/v1/:deploymentId/assignments/party/:partyId \
URL (groups): https://api.epicgames.dev/epic/avatar/v1/:deploymentId/assignments/groups \
Method: GET \
Auth Required: Yes (Account Auth)

## Path Parameters

`deploymentId`: `9c9906b240c74a92a6b9100d6e4ccbd0` <br/>
`partyId`: The Party Id (party route only)

## Query Parameters

`accountId`: Optional, comma separated Account Ids to limit the result (friends: without it all friends are returned) <br/>
`conversationId`: Comma separated group chat Conversation Ids (groups route only)

---

_Example Response (friends, shortened)_

```json
{
  "assignments": [
    {
      "accountId": "94b1569506b04f9f8557af611e8c5e47",
      "avatar": {
        "avatarId": "AthenaCharacter:cid_defaultoutfit[2,13]",
        "url": "https://cosmo.fdeb.live.use1a.on.epicgames.com/cdn-cgi/image/height={},format=png/v1/item/WER5RlAYhxo-8yifvRDInC-Q2XrexQd5yOUDL4gAPA4/png"
      }
    }
  ]
}
```

_Example Response (party / groups with no match)_

```json
{
  "assignments": [],
  "failedAccountIds": []
}
```
