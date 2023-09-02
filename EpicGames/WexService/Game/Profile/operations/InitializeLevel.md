# InitializeLevel

**Description**: `Initializes and starts a level` \
**Profiles**: `levels`

## Body

```js
{
    "manifestVersion": "", // Client Content Version (body varies significantly between some versions)
    "levelId": "", // ID of Level to Initialize
    "partyId": "", // GUID of active party (old versions only)
    "partyMembers": [ // New versions only
        {
            "heroType": "", // Type of Party Member (e.g. LocalHero, FriendCommander)
            "heroItemId": "" // GUID of Hero
        }
    ],
    "commanderId": "", // GUID of selected friend commander (old versions only)
    "friendInstanceId": "", // Friend Instance GUID (for friend commander)
    "ltmId": "", // ID of the active LTM for the zone (new versions only)
    "normalMode": true, // Challenge Mode (new versions only)
    "blitzMode": false, // Unused, blitz levels are not playable in later versions (new versions only)
    "teamPower": 364155 // Combined Hero Power (new versions only)
}
```
