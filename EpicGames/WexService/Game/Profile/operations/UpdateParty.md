# UpdateParty

**Description**: `Updates a party's data` \
**Profiles**: `profile0`

## Body

```js
{
    "partyItemId": "", // GUID of the party instance to update
    "partyInstance": {
        "character_ids": [
            "" // GUID of heroes in the party
        ],
        "pet_id": "", // GUID of the pet in the party (old versions only)
        "friend_index": 1, // Index in the party for a friend commander
        "commander_index": 0, // Index in the party for the player's commander
        "date_created": "2019.11.13-07.11.54", // Date the party was created
        "party_icon": "None" // Icon assigned to the party
    }
}
```
